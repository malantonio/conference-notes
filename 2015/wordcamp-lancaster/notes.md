## building parsec (responsive themes) - [joe casabona](http://casabona.org) ##

* [slides](rwdwp.com/102)
* [parsec theme](github.com/jcasabona/parsec)

* sketch
    * have an idea of what it'll look like
* style tile
    * essentially a style guide / mockup
    * view how everything looks
    * using photoshop
    * [styletil.es](http://styletil.es)
* _s as base
* _using inline svg_ book
* breakpoint decisions
    * use min-width rather than max-width -- mobile first
* ~~is he saying RESS? or REST? for responsive loading~~
    * (it was RESS)
* wp galleries w/ figure + figcaption: `add_theme_support( 'html5' )` ?

## macaw + responsive themes - Tim McKenna ##

* macaw => nah dawg: just stick w/ the long way
* maybe more production functionality w/ 2.0 (slated for august)

## genesis framework: hooks + filters for theme dev [Sarah Moyer](http://sarah-moyer.com) ##

* premium theme ($60)
* uses/adds custom action + filter hooks
* adds only 2 settings pages in admin
* building-block-esque development: blocks of content

* moving nav bar to the top:
    remove_action( 'genesis_after_header' , 'genesis_do_nav' );
    add_action( 'genesis_before_header', 'genesis_do_nav' );

* filter hooks to change pieces of content

## css, the exciting parts - [Beth Soderberg](http://bethsoderberg.com) ##

### transforms ###

* use browser prefixes!
* manipulating items on the dom
* can include multiple transforms in a line
    * matrix has a _ton_ of possibilities
* ex:
    * `rotate`
        * positive right, negative left (clockwise)
        * `transform: rotate(#degs)`
    * `scale`
        * bigger/smaller
        * `transform: scale(valueX[, valueY])`
            * just X assumes duplicate for Y
    * `skew`
        * "swooshy shapes"
        * `transform: skewX(angleX)`
            * preferrable to skew individual axis vs. both a la `transform`
    * `translate`
        * move a thing from over here to over there
        * `transform: translate(valueX[, valueY])`
            also `transformX` + `transformY`
* more efficient re: browser performance
* transform origin
    * default  `transform-origin` is 50% 50%
    * `transform-origin: x-offset y-offset`
        * diff. units, keywords, etc.
* prefix requirements:
    * `-ms-`
    * `-webkit-`

### transitions ###

* transition from one property to another (think `:hover`)
* properties
    * `transition-property`
        * specifies which properties are impacted by transition
        * 'property names': css properties: width, color, font-size, etc.
    * `transition-duration`
        * how long for transition to take effect
    * `transition-timing-function`
        * pace at which yr animation is run
    * `transition-delay`
        * wait to trigger (useful in animations)

* ie support only 10+
* requires `-webkit` prefix

### animations ###

* keyframes!
    * establish the behavior of an animation over time
    * percentages, or `from` + `to`
* properties
    * `animation-duration`
        * length of time for one cycle of yr animation
        * accepted in seconds `s` or milliseconds `ms`
    * `animation-name`
        * custom value to define yr animation (no spaces!)
    * `animation-iteration-count`
        * number, infinite, initial, inherit
* not all css properties are 'animatable'
* `animation-play-state`
* ie support only 10+
* check out the working drafts @ `w3.org/TR`

* `@bethsoderberg`
* `bethsoderberg.com/slides/2015/wordcam-lancaster`

## version control for freelancers + small teams - [Liam Dempsey](http://lbdesign.tv) ##

* [slides](http://bit.ly/wclanc)

## using backbone - [Nick Smith](http://10up.com/) ##

* backbone vs. jquery
    * bb more data-driven (?)
* bb used in wp core
* use nonce fields!
* include backbone by adding `'backbone'` to enqueue_script dependencies array
* `wp_send_json_error()` function

## documentation is for everybody - [Jeff Matson](http://jeffmatson.net) ##

* use visuals (pictures / videos)

## get involved! (in non-code ways!) ##

* [make.wordpress.org](http://make.wordpress.org)
* [chart used](https://twitter.com/wplanc/status/571767628886360064)
* [amara](http://amara.org) to caption / subtitle videos
* [slides](http://slides.thetracyl.com/wclanc2015/)

## open source schoolhouse ##

* koha library system
* own cloud
* [github.com/pennmanor](http://github.com/pennmanor)
* "our jobs as educators is to make our jobs obsolete"