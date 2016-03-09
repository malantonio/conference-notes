[Visualizing Solr Search Results with D3.js for User-Friendly Navigation of Large Result Sets] - Julia Bauder
-------------------------------------------------------------------------------------------------------------
* _seeking meaning: a process approach to library and information services_, c.c. kuhlthau (2004)
* search results as list, way too much information to process
* solr's got facets + pivot facets (facets w/in facets)
* https://github.com/mbostock/d3/wiki/gallery -> examples of d3 visualizations
* d3 expects data that isn't quite how solr spits out pivot data, fix on github
* d3 has good support for json; color schemes built in
* ["thinking with joins"](http://bost.ocks.org/mike/join/‎) by mike bostock, helpful article on d3
* grinnell college library github

[Visualizing Library Resources as Networks] - Matt Miller
---------------------------------------------------------
* nypl labs
* michel foucault, _the archaeology of knowledge_
* 'serendipity' -> finding something you didn't know you wanted
* http://archives.nypl.org/mss/2993
* has to operate in browser, a lot of heavy lifting
* need access terms, time-consuming
* in the catalog 'each subject heading is a node in the graph, including subdivisions'
* 'the size of the node is determined by the nuber of occurrences'
* http://bit.ly/nyplnetwork -> self-organized map of nypl subject headings
* organized by their use in records
* uses [gephi toolkit](https://gephi.org/toolkit), pymarc
* https://github.com/thisismattmiller/catalog-network

[We Are All Disabled! Universal Web Design Making Web Services Accessible for Everyone] - Cynthia Ng
----------------------------------------------------------------------------------------------------
* http://bit.ly/c4l14-arty
* assistive technology
* 'all technology is assistive technology' - @ablerism
* 'there is no average user.'
* universal design -> usable by all people
* for web:
    * consistent navigation
    * meaningful order to content
    * multiple ways to discover content (menu bar/ search box)
* key strategies
    * mobile first
    * progressive enchancement
    * responsive design
* alt text
* 'say NO to autoplay'
* 'death to the carousel'
    * not keyboard accessible
    * shouldiuseacarousel.com
* tab key should get you thru the site in order
* skip to menu button
* aria (accessible rich internet application suite)
    * role="..."
    * http://w3.org/TR/aria-in-html
* http://a11yproject.com
* http://validator.w3.org
* html code sniffer
* WAVE toolbar
* __screen-reader emulators__
* human guidelines
    * use headers properly
    * use descripted links
    * describe your images
    * embed auidio/video, add a link to original
* 'universal usibility is simply good design'
* @TheRealArty
* hard to automate, ask yr users again and again

[Dead-simple Video Content Management: Let Your Filesystem Do The Work] - Andreas Orphanides
--------------------------------------------------------------------------------------------
* the problem: content management
    * too many files in video webspace
    * lots of work repetition (a lot of repeated code)
* the solution: content management
    * two scripts for video playback
    * videos/metadata stored remotely (different directory)
    * content layer + display logic separate
    * videos and metadata stored together
* http://server/myvideo
* script goes to video server in /myvideo directory
* it's mvc!
* .mp4, .webm
* directory exists = file exists
* no xml file? splits filename into title -> fallback
> * limitations
>   * discovery challenges - indexing
>       * solution: gallery page
>   * metadata limitations - categories, etc.
>       * solution: ???
>   * content creators not isolated from system
>       * webforms, etc?
>   * compatibility with content management policy / practice?
>       * technical integration _should_ be straightforward
* code is on dropbox

[Bulding for others (and ourselves): the Avalon Media System] - Michael B. Klein and Julie Rudder
-------------------------------------------------------------------------------------------------
* hydra-based manager of digital audio/video
* ingest + describe content; media transcoded, indexed
* lti -> learning tools interoperability
* 'lti should work well with any system that supports lti'
* puppet -> administrative deployment tool.
* http://avalonmediasystem.org

[Sustaining your Open Source project through training] - Bess Sadler and Mark Bussey
------------------------------------------------------------------------------------
* http://projecthydra.org
* http://railsbridge.org
* dive into hydra (similar format to railsbridge)

[Behold Fedora 4: The Incredible Shrinking Repository!] - Esmé Cowles
---------------------------------------------------------------------
* https://github.com/ucsdlib/damspas (_not_ fedora)
* https://github.com/futures/fcrepo4 (alpha)

[A reusable application to enable self deposit of complex objects into a digital preservation environment] - Jill Sexton, Mike Daines, and Greg Jansen
------------------------------------------------------------------------------------------------------------------------------------------------------
* 'an app that lets non-programmers develop webforms and map plain text labels to MODS elements'
* https://github.com/unc-libraries/deposit-forms

[Organic Free-Range API Development - Making Web Services That You Will Actually Want to Consume] - Steve Meyer and Karen Coombs
--------------------------------------------------------------------------------------------------------------------------------
* ncip standards
* oauth(2) means opt-in

[Towards Pasta Code Nirvana: Using Javascript MVC to Fill Your Programming Ravioli] - Bret Davidson
---------------------------------------------------------------------------------------------------
* http://go.ncsu.edu/js-mvc
* spaghetti code
* lasagna code: many layers, maybe too many dependencies
* ravioli: modular code, fewer dependencies
* 'modular, reusable, testable'
* _tao of programming_
* three pilars of using js
    * js is everywhere
    * js is fast
    * js is the lingua franca
* approximate architecture, models, views, controllers, data binding
* can result in _not_ touching selectors again
* **when to use?**: 'js heavy apps, interactive apps, distributed, modern devices/browsers'
* **when to avoid?** 'need to support no-JS users, app is document driven (blog), older devices/browsers'
* popular: angular, ember, backbone
* http://todomvc.com
* https://github.com/cazzerson/Suma
* end goal: 'make applications that help library users'

[PhantomJS+Selenium: Easy Automated Testing of AJAX-y UIs] - Martin Haye and Mark Redar
---------------------------------------------------------------------------------------
* python + ruby ('gem install selenium')
* firefox, chrome, ie, phantomjs
* selenium ide records user actions on a page
* virtualenv -> simulates blank python install 
* phantomjs -> headless web browser, speeds up test (doesn't have to open a browser)
* saucelabs browser tests in the cloud
* https://github.com/mredar/code4lib-2014-phantomjs-selenium

[Queue Programming -- how using job queues can make the Library coding world a better place] - Birkin James Diana
-----------------------------------------------------------------------------------------------------------------
* job queues good for 'long-running jobs, responsivenes & scalability'
* 'job' -> call to a function + data it needs

[Visualizing Solr Search Results with D3.js for User-Friendly Navigation of Large Result Sets]: http://code4lib.org/conference/2014/bauder
[Visualizing Library Resources as Networks]: http://code4lib.org/conference/2014/miller
[We Are All Disabled! Universal Web Design Making Web Services Accessible for Everyone]: http://code4lib.org/conference/2014/ng
[Dead-simple Video Content Management: Let Your Filesystem Do The Work]: http://code4lib.org/conference/2014/orphanides
[Bulding for others (and ourselves): the Avalon Media System]: http://code4lib.org/conference/2014/klein
[Sustaining your Open Source project through training]: http://code4lib.org/conference/2014/sadler
[Behold Fedora 4: The Incredible Shrinking Repository!]: http://code4lib.org/conference/2014/cowles
[A reusable application to enable self deposit of complex objects into a digital preservation environment]: http://code4lib.org/conference/2014/sexton
[Organic Free-Range API Development - Making Web Services That You Will Actually Want to Consume]: http://code4lib.org/conference/2014/meyer
[Towards Pasta Code Nirvana: Using Javascript MVC to Fill Your Programming Ravioli]: http://code4lib.org/conference/2014/davidson
[PhantomJS+Selenium: Easy Automated Testing of AJAX-y UIs]: http://code4lib.org/conference/2014/haye
[Queue Programming -- how using job queues can make the Library coding world a better place]: http://code4lib.org/conference/2014/diana