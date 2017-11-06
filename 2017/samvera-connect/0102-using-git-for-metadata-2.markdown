using git for metadata, pt. 2
=================

(git + github + the metadata flow)

- alex dunn
- matt critchlow
- chrissy rissmeyer

- uc santa barbara
- uc san diego

-----

- lynda.com git tutorial as training

- ucsb, repo on public github, metadata on enterprise github
- wednesday session 
  - Wed 11:35 – 12:05  Session 5  GRAND PARLOUR - C
    - Metadata management and batch ingest automation with Git/GitHub,
      Jenkins, Ansible, and JIRA
- central repo for metadata, folders for projects

- metadata providers?

- what does a good commit message look like (for metadata)?

- editing metadata for the repo in an excel way + then side ingest
  in an automated way?
- metadata validation tests to be run on pull-requests
  - how are the validations being run?
  - using jenkins
  - https://github.com/ucsblibrary/metadata-ci
- then pulled into a qa environment before pushing to production

- eventually pushes onus on batch-ingest to metadata librarian
- eventually would like to use ui interface to edit items
  - a good strategy for in-process

- yr staging environment should be a close mirror of production

- metrics? low bar of requires on the application side, impose business rules
  - per-project schema
  - field counts

- no real plan for post-ingestion (which is where you're at!)
- make metadata available for public access?

- csv, marcxml, mods <-- input
- triples <-- output

- found to be a benefit for migration bc you'll need to ingest multiple times
  - BUT TAKE IT DOWN AFTER <~ it can become a crutch + you'll have to edit it
    in two places

- https://github.com/ualbertalib/metadata

