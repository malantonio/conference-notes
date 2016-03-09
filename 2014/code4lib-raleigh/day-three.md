
Closing Keynote - An Interview with [Valerie Aurora]
----------------------------------------------------
* 'imposter syndrome' training
* ada camp, differing colored lanyards to denote: ok to take picture, ask for permission, no pictures
* mansplaining
* 'hackerspace' -> 'community workshop'
* anil dash article re: retweeting only women
* different, global term for 'programming', 'coder' -> 'software creator'
* inclusive rather than exclusive: 'all-gender' bathrooms vs. 'gender-neutral'

[Under the Hood of Hadoop Processing at OCLC Research] - Roy Tennant
--------------------------------------------------------------------
* apache project for parallel processing
    * hadoop coor
    * h. distributed file system
    * hbase - h database
    * pig - high-level data-flow language
* MapReduce
    * mapping - filtering + sorting: "find all the ____ with ____"
    * reducing - merging + summarizing: do something w/ the results
* hadoop manages behind the scenes stuff
* java native
* can use any language w/ 'streaming' option ( could pass mappers + reducers in different languages )
* hbase useful for accessing it as a database
* hangingtogether.com blog
* worldcat linked data explorer
* http://roytennant.com

[Lucene’s Latest (for Libraries)] - Erik Hatcher
------------------------------------------------
* http://code4lib.org/conference/2013/hatcher
* apache solr reference guide 4.x
* http://blog.mikemccandless.com

[All Tiled Up] - Mike Graves
----------------------------
* spherical mercator / web mercator
* zoom-level | resolution / colum / row
* basic web gis stack
    * tile cache
    * ogc endpoint
    * geodatabase
* https://github.com/mapbox/mbtiles-spec
* strores map data in sqlite db
    * metadata   | tiles
      -----------|-------------
      name       | zoom_level
      value      | tile_column
                 | tile_row
                 | tile_data
* https://github.com/mapbox/tilemill
* open geoportal


[Valerie Aurora]: http://blog.valerieaurora.org/
[Under the Hood of Hadoop Processing at OCLC Research]: http://code4lib.org/conference/2014/tennant
[Lucene’s Latest (for Libraries)]: http://code4lib.org/conference/2014/hatcher
[All Tiled Up]: http://code4lib.org/conference/2014/graves