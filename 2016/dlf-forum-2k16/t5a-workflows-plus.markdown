Practical Options for Incoming Digital Content
==========

**presenters:** Jody DeRidder, Alissa Helms

- https://osf.io/qprn4
- dig content intake
	- identification
	- analysis
	- selection
	- processing
- forensics toolkit (ftk)
	- $$$$
- top formats
	- pdf for text
	- tiff for image
	- wav for audio
	- mp4 for video
- forthcoming november d-lib has article about this
- 

Designing User-Friendly Ingestion Workflows
==========

**presenter:**  Eli Zoller (+ Sarah Sweeney)

- 6 "loaders"
	- iptc photograph loader
		- zip file of jpgs
		- metadata extracted from uptc header + translated to MODS
		- allows users to add metadata in their own tools + not tied to the website
	- multipage loader
		- lib staff - originally designed around a specific lib collection
		- zip of images + their associated mods xml metadata
		- loads sequential images for objects like postcards + page images (via csv?)
	- xml loader (metadata + files)
		- for new objects
		- archives + special collections and library staff
		- zip file of files + MODS xml
		- loads new files w/ their associated metadata
	- xml loader (metadata only)
		- updating (not loading new items)
		- zip file of mods xml
		- replaces existing mods xml w/ provided file
	- spreadsheets (metadata + files)
		- zip file of files + excel file
		- loads new files w/ their associated metadata by transforming spreadsheet
		  metadata into mods xml
	- spreadsheets (metadata only)
		- zip file only contains excel file
		- updating (not loading new files)
- loaders presented to users based on roles
- after uploaded, passed to "load report" which shows status of processing
	- notifies if metadata was changed
- spreadsheet flow
	- (google) form is filled out, spreadsheet is automatically generated, then 
	  quality control applied to spreadsheet (as opposed to MODS), before being
	  uploaded
- less training / lower barrier quality control

Snapshot - Library Workflow Exchange: Community Documentation of Best Practices
==========

**presenters:** Liz Woolcott, Anna Neatrour

- libraryworkflowexchange.org
- "i wonder if anyone else has done this before?"
	- "someone, somewhere is doing (almost) the same thing you are"
- @LibWorkflowEx

Snapshot - “Does the Research Generate Data?” and Other Ambiguous
==========

**presenters:** Elizabeth Bedford, Greta Pittenger

- "one size does not fit all for workflows"
