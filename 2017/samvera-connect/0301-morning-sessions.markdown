morning sessions
================


lightning talks - a
-------------------

- honeybadger
  - https://honeybadger.io

-----

- embedding works
  - https://github.com/sul-dlss/sul-embed

-----

- using student workers for qa?
- give students work they can accomplish in a day
  - break things into small chunks

- involve students in meetings when possible
- helps w/ documentation

-----

- netdata
  - netdata for server monitoring
  - https://my-netdata.io
  - https://github.com/firehol/netdata

-----


Collections Extensions and Admin Sets: Flexible approaches to grouping things in the repository
----------

- e. lynette rayle @ cornell

-----

- hoping for release in hyrax 2.1
- checkout the `collections-sprint` branch to try it out
- nesting of collections allowed
- adds 'managed collections' tab which allows granted users to work
  on collections
- collections w/ sub-collections don't show all of the sub-items
- search in collection w/ sub-collections only shows that collection's top level
- possible to change this?

-----


Our Journey from Sufia 7 to Hyrax
--------------

- Glen Horton
- Thomas Scherz
- Sean Crowe

-----

- scholar@uc - self-deposit
- https://github.com/samvera/hyrax/releases/tag/v1.0.1
  - instructions for upgrade from sufia 7.3 -> hyrax 1.0.1
- rails 5, ruby 2.4
- migration commits
  - https://github.com/uclibs/scholar_uc/commits/6b479d2189950e6efed40d4f93f805a332ee9e1e
- pull-request
  - https://github.com/uclibs/scholar_uc/pull/1393
- has bulk ingest tool built in
- https://scholar.uc.edu/
- to get files out of fedora pulled from the filesystem after identifying
  (instead of using the apis)
  - used checksums (3x)
- see repo/wiki for data migration info (forthcoming)


How are people using workflows and Admin Sets in production Hyrax systems?
----------

- steve van tuyl

-----

- ted talk performance art w/ av breaking

- no one will know what 'relationships' means
- use admin sets to determine workflows
- resource type
  - metadata field (the dropdown)
- "work type is less granular kind of thing"
  - ex. scanned resource (work type), photograph (resource type)
- use work type to define different metadata fields
  - but may need to define multiple similar work types to prevent having to 
    explain resource types
- workflows defined w/ a json file
  - recco build a diagram when building a workflow.json file to better
    visualize the workflow
  - also _test it_


Metadata management and batch ingest automation with Git/GitHub, Jenkins, Ansible, and JIRA
------------

- Alex Dunn
- Chrissy Rissmeyer

-----

- slides
  - https://docs.google.com/a/lafayette.edu/presentation/d/1137S5BikGclUUOKavZsveHDACdH6iIUXAP5PW918jPc
- adrl
