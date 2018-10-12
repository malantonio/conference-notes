The Guardian Workflow: a generalized approach for integrating Amazon Glacier with a Samvera repository
-------
Kate Lynch

- https://github.com/upenn-libraries/stronghold
- https://github.com/upenn-libraries/guardian
- https://github.com/upenn-libraries/guardian_manifest
- https://github.com/upenn-libraries/todo_runner

glacier terms
====

- regions
  - physical region of glacier store
- vaults
  - grouping mechanism for archives
  - think s3 buckets
  - limit of 1,000 vaults per account per region
- archives
  - immutable individual unit of data durably sotred in a vault
  - upt to 100tb in size
  - archive id
  - one piece of additional metadata
  - recommended to group (via tar)
- inventories
  - manifest of contents of a vault
  - downloadable as json or csv
  - async: request + in about 3hrs you'll get a doc

best practices w/ glacier
=====

- record archive metadata somewhere (else)
- be mindful of proliferating jobs
  - recommended to coordinate who's getting what when
- only request what you can retrieve
  - downloadable for 24 hours
  - network constraints
  - available storage
- pick a region that isn't absolutely near you

- git-annex for large file validation?


considerations for large-scale disaster recovery
=====

- glacier region
- prioritized retrieval
- metadata-only archive
- application-specific vaults

