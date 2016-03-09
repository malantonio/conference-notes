# how to avoid mucking up yr dns (sal ferrarello / @salcode)

* `dig` to read from nameservers
* CNAME is cononical name => akin to "see also ..."
* make sure to include the trailing period for Fully Qualified Domain Name
    www.bummer.website.  => FQDN
    major                => relative, points to major.bummer.website.
    major.bummer.website => relative, points to major.bummer.website.bummer.website.
* get nameservers
  * `dig NS <url>`
* query a nameserver directly
  * `dig <url> @<nameserver address>`

To recap:

    IP Address   | phone number
    A Record     | phone listing (name to number)
    CNAME record | name change listing
    TTL          | how long a DNS value is cached

* http://salcode.com/love-dns

# unicode (casey driscoll)

* see http://caseydris.co/wclanc16

# learn to love the terminal (brad parbs / @bradp gh / http://brad.party)

* http://explainshell.com
* http://shellcheck.net
* `tig` (`brew install tig`)

# you have something to say (tracy rotton / @taupecat)

* taupecat.github.io/you-have-something-to-say
* https://make.wordpress.org
* https://wordpress.tv

# let's learn about the wp rest api (ty fujimura / http://cantilever.co)

* https://github.com/tyfuji/wp-api-demo

# 'open source everywhere' panel

* codeforphilly.org
* schoolpress.co
* open source as a sharable recipe
* "program or be programmed" - book
* richard stallman ted talk
* "the cathedral and the bazaar"

# misc / note-to-self

* go to wordpress.tv to watch "outgoing on command" talk
