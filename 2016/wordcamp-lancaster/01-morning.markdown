# making the magic happen with wp-cli (ryan duff)

* use wp-cli for scripting tasks
  * (maybe you should automate whipping up dummy sites?)
* can you post from cli?
  * yup! http://wp-cli.org/commands/post/create/
    * flags mirrored from wp_insert_post $postarr parameter
      * https://developer.wordpress.org/reference/functions/wp_insert_post/
    * pipe html in or use a file; pass categories/tags as flags

# organizing yr first website usability test (anthony paul (@anthonydpaul / http://adp.rocks))

* usability !== user test
  1. user focus is best practice
  2. validate client assumptions
  3. inform yr design deciions
  4. show success over time
  5. grow as a practitioner (e.g.  hamburger icon)

* 'The designer-loved hamburger icon is not universally understood.'

## what you need

----------------|-------------
project goal    | a reson to test, to be translated into research goals
test strategy   | when to test and what type of test(s)
prototype       | or, other artifact
test facility   | hardware, software, or physical space
participants    | demographics, if relevant

- project goal
  * why are we working on this?
    * university => prospects to easily find degree info
    * e-store => reduce shopping cart abandonment
    * non-profit => drive donations
  * ok to have multiple goals

- test strategy
  * 'project constraints + hariest problems (priorities) = maximum benefit'
    * project constraints
      * # of sets of tests, usually 8-12 tests/participants
    * harriest problems
      * too much content
        * test info architectrue or interactive menu concepts
      * (vs) brand perception is important
        * test design concepts, photography, and copywriting

* TryMyUi ($35 per video) / usabilitytesting.com
* run test on early designs or wireframes
  * use invisionapp.com, draw links/functionality by uploading screenshots/design layouts
* pilot test with a friend to get a sense of timing
* TryMyUi works in a mechanical-turk way: hires outside users (can select diversity)

# pushing yr development skills: learn by doing it (sarah moyer)

* (slick js library: http://kenwheeler.github.io/slick)

# understanding security holes (george stephanis (http://stephanis.info))

* cross-site request forgery (csrf)
  * send nonce (Number used ONCE)
  * wp nonce generated from:
    * current 12 hour tick
    * action name
    * user's ID
    * session token
  * nonces for intent, _not_ authentication: making sure request came from the site

* cross-site scripting (xss)
  * injecting/executing malicious javascript
  * use `esc_attr` and the like liberally
  * restricted to the scope of the logged-in account that's being hijacked

* sql injection (sqli)
  * use prepared statements!!! `$wpdb->prepare()`
  * whitelist values (if $val == "this_thing" ... if $val == "that_thing" ...)
  * "sanitize early / escape late"
    * sanitize == understanding content
    * escaping == understanding context

* maybe don't fully go into the security breach in the commit message?
* `sanitize_text_field()`

# tiptoe through the templates (reed gustow)

* `wp_nav_menu()`: useful for social links
