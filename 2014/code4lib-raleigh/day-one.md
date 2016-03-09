Opening Keynote - [Sumana Harihareswara]
----------------------------------------
* lib that logs everytime they have to tell a patron 'no'
* empathy in ux
* userslib.com

[A Book, a Web Browser and a Tablet: How Bibliotheca Alexandrina’s Book Viewer Framework Makes it Possible] - Engy Morsy
------------------------------------------------------------------------------------------------------------------------
* storage -> image/content processing -> search/personalization/metadata/copyright (determines on/off campus access) engines
* http://dar.bibalex.org

[Quick and Easy Data Visualization with Google Visualization API and Google Chart Libraries] - Bohyun Kim
---------------------------------------------------------------------------------------------------------
* google visualization api query language -> google chart libraries
* able to search spreadsheet like sql
* developers.google.com/chart/interactive/docs
* js: google.visualization.Query class
* slideshare.net/bohyunkim
* github.com/bohyunkim/examples
* bohyunkim.net/blog

[WebSockets for Real-Time and Interactive Interfaces] - Jason Ronallo
---------------------------------------------------------------------
* ncsu digital collections
* github.com/jronallo

[Personalize Your Google Analytics Data with Custom Events and Variables] - Josh Wilson
---------------------------------------------------------------------------------------
* 'custom dimensions' in new beta Universal Analytics
* github.com/joshwilsonnc/ga_cdm (contentDM GA script)
* HTTPFox (for firefox)
(what about a 'tracking' extension/add-on that stores staff credentials to disregard??)

[Discovering your Discovery System in Real Time] - Godmar Back and Annette Bailey
-------------------------------------------------------------------------------
* embedded js, records click, uses api to get item (summon ids change) then stores in db

[Structured Data NOW: seeding schema.org in library systems] - Dan Scott
------------------------------------------------------------------------
* 'scalable structured markup' google i/o talk
* http://schema.org
* worldcat schema.org json extension
* openstreetmap
    "
    persistent uris
    html5
    rdfa expressing schema.org
    sitemaps listing uri of interest
    "
** w3c library linked data incubator group report **
* "2012 common crawl"
* RDFa/RDFa Lite
* 'structured data linter'
* w3c schema bib extend community group (SchemaBibEx)
* map holdings to schema.org offers (seller items)
* stuff.coffeecode.net/2014/structured_data_now

[Next Generation Catalogue - RDF as a Basis for New Services] - Anne-Lena Westrum, Benjamin Rokseth, Asgeir Rekkavik, and Petter Goksøyr Åsen
---------------------------------------------------------------------------------------------------------------------------------------------
* stepping away from marc
* 'digital mediation center'
* v. useful for physical collections
* patron has to choose edition according to title (to user, all are the same!)
* opac doesn't realize books are the same
* adding common sense to data, no room in marc for that
* marc2rdf toolkit (open source)
* github.com/digibib/marc2rdf -> expressing marc ~~records~~ data as rdf statements
* deichmanske bibliotek
* maps marc to fields ( json/yaml esque )
* sparql language
* http://github.com/digibib
* http://digital.deichman.no

[More Like This: Approaches to Recommending Related Items using Subject Headings] - Kevin Beswick
-----------------------------------------------------------------------------------------------
* collaborative filtering / content-based filtering
* interested b/c popular sites use it, users come to expect it
* good for items _not_ shelved next to each other but similar in topic
* also for e-books that don't have call numbers
* match on most subject headings (produces decent recommendations)
* match on first subject headings (work down until enough results/run out) (produced too few results)
* match on most subject terms (vs entire heading)
* match on weighted subject terms (geographic, subdivisions, chronological, etc.) (differs on subject or user's interests, don't want user input)
* python handles requests / solr does heavy lifting
* solrmarc library (marc fields loaded into solr)
* solr assigns scores?

[Sumana Harihareswara]: http://www.harihareswara.net/
[A Book, a Web Browser and a Tablet: How Bibliotheca Alexandrina’s Book Viewer Framework Makes it Possible]: http://code4lib.org/conference/2014/omar
[Quick and Easy Data Visualization with Google Visualization API and Google Chart Libraries]: http://code4lib.org/conference/2014/kim
[WebSockets for Real-Time and Interactive Interfaces]: http://code4lib.org/conference/2014/ronallo
[Personalize Your Google Analytics Data with Custom Events and Variables]: http://code4lib.org/conference/2014/wilson
[Discovering your Discovery System in Real Time]: http://code4lib.org/conference/2014/back
[Structured Data NOW: seeding schema.org in library systems]: http://code4lib.org/conference/2014/scott
[Next Generation Catalogue - RDF as a Basis for New Services]: http://code4lib.org/conference/2014/westrum
[More Like This: Approaches to Recommending Related Items using Subject Headings]: http://code4lib.org/conference/2014/beswick