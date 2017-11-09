afternoon sessions
==================

APIs, Sharing Work, Specifications and Alternative Data Stores
-------

- Trey Pendragon
- Benjamin Armintor

-----

- community notes
  - https://docs.google.com/document/d/1a3aV2Mck8SWj3gQ4LyyUoViJKwO-gLWq2BQMfH2MQn4


-----


Moving to AWS
-------------

- Erin Fahy
- Don Brower
- David Schober
- Michael Klein
- Carolyn Caizzi
- Hannah Frost

- (northwestern + stanford)
- (( notre dame is looking @ it ))

-----

- slides
  - https://docs.google.com/presentation/d/1amcIx3YMEUyYn6ZedPblQiXkaK4QAlKE70F2poDR104
- "infrastructure as code (staging, dev, prod are identical)"
- ephemeral servers!
- no local storage! (no tmp files)
- yo ephemeral storage is crayyyyzzzy
- + no local deploys needed, can "just refresh a bookmarked url"
- "expanded access to file services"
- "are mission critical services better in the cloud?"
- reduced workload on devops staff 🎉🎉🎉
- travis has deployment tools for green checks
- "code pipeline" / beanstalk
- cloud will be $$ but how about what our costs are now
- how do you know that this deployment is ok for this environment
- gem install `okcomputer`
  - adds a `/status` url that can be used to check
- shipping configuration w/ code
  - `.eb` extensions directory
- can treat aws as a vm farm _or_ rewrite to embrace its services
- "how do you handle secrets?"
- "so many aws services, difficult to choose the right one"
- nd has preservation tape storage on campus, how to save things there
  + cache(?) in the cloud

- understand beanstalk + how it works
- github -> ci greenlight -> deploy (code-pipeline -> beanstalk)
- cloudformation
- don't try to deploy everything at once!! piece by piece
  - fedora
  - postgres
  - solr
  - etc.
- "can't assume anything about the environment"
- rails-config can take env variables, which allows you to set settings
  in aws but also use a local dev environment

-----

Samvera stack in production the DevOps way
--------------

- Kieran Etienne
- Erin Fahy

-----

- be super clear abt what you're planning to do before coding
- "blue/green deployment" -> comes from aws land
- capistrano
- ansible / chef / puppet
- netdata
- rollbar (?)
- graylog (open source log aggregator)
- terraform
- https://github.com/devops4lib
