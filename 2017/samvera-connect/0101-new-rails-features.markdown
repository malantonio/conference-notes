New Rails features and how to use them - Rob Kaufman
===========

- slides: https://bit.ly/2hgH0Ae
- @orangewolf
- notch8.com

----

- `ActiveJob`
  - http://guides.rubyonrails.org/v5.1/active_job_basics.html
  - uniform instance for background work
  - "active record like interface for jobs"
  - code runs outside typical request
  - can be backed by different bg runners: DelayedJob, Resque, Sidekiq Built
    in queue
- `ApplicationRecord`
  - adds a parent object that all models inherit from
  - makes AR uniform with ApplicationControllers
  - Applies to ActionMailers + ActiveJob
  - (parent class for Models to inherit from)
- Attributes API
  - gives types to `attr_accessor` or AR atribute objects
  - you can add yr own custom types
  - 'hey im storing this as a text blob but its really an array'
- wEbPaCkEr (new in rails 5.1, april '17)
  - brings in webpack + yarn
  - (they're kinda off wrt js info but whatever // lone js in a room of
    rubyists)
- `ActionCable`
  - Websockets in Rails
  - Can create realtime updating events + access them on server/client side
  - uses PubSub for clients

- AcTiVe JoB
  - be sure to test that yr async job actually does the job + doesn't pretend
  - http://api.rubyonrails.org/v5.1.4/classes/ActiveJob/QueueAdapters.html

```ruby
# bin/rails generate job guests_cleanup --queue urgent

class GuestsCleanupJob < ApplicationJob
  queue_as :urgent

  # prefer ordered arguments?
  def perform(*guests)
    # do something later
  end
end

# configure it
# config.active_job.queue_adapter = :sidekiq
```

```ruby
GuestsCleanupJob.perform_later guest

# ~~or~~

GuestsCleanupJob.set(wait_until: Date.tomorrow.noon).perform_later(guest)

# ~~or~~

GuestsCleanupJob.set(wait: 1.week).perform_later(guest)

# ~~or~~

GuestsCleanupJob.perform_later(guest1, guest2, filter: 'some_filter')
```

callbacks

- `{before,around,after}_enqueue`
- `{before,around,after}_perform`

- don't store an object in the queue, just use the id (via `before_enqueue`)

-----

exercise
--------

- move the following to background tasks
  - sending an email report from SearchRecord once a day
  - creating a SearchRecord when a search is done

-----

- restart yr workers (redis / whatever) when you update the code!!
- maybe chain jobs within other jobs _but make sure you check to see if it's
  already been called!!_

-----

- attributes!

```ruby
attribute :start_date, :date, default: -> { 1.day.from_now }
attribute :end_date, :date, default: -> { 8.days.from_now }
```

- types! `app/types`

```ruby
# app/types/price.rb
class PriceType < ActiveRecord::Type::Integer
  def cast(value)
    return super if value.kind_of?(Numeric)
    return super if !value.to_s.include?('$')

    price_in_dollars = BigDecimal.new(value.gsub(/\$/, ''))
    super(price_in_dollars * 100)
  end

  # can also do something on the way in
end
```

```ruby
# config/initializers/types.rb

ActiveRecord::Type.register(:price, Price)
```

useful for currency conversions

-----

wEbPaCk
-------