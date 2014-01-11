---
layout: post
title: "Jasmine Maven Plugin 1.3.1.0 - My first release"
author: klieber
date: 2013-03-12 23:57:41.000000000 -05:00
categories:
- Development
- JavaScript
tags:
- JavaScript
- maven
- testing
- jasmine
- open source
comments:
- id: 152
  author: Jeremy Robin
  author_email: jeremy@jrob.co
  author_url: http://www.rolloco.com
  date: !binary |-
    MjAxMy0wNC0xNiAxNjo1NToyNiAtMDUwMA==
  date_gmt: !binary |-
    MjAxMy0wNC0xNiAyMTo1NToyNiAtMDUwMA==
  content: ! 'Just wanted to thank you for the work you''ve been putting in to the
    jasmine maven plugin.


    i went to the github site today and saw that the new plugin version with phantomjs
    was up.  BOOM.  100% of our tests passing from the command line (with htmlunit
    it was about 50%).  we can now put our jasmine tests back in the test goal so
    they run as part of our jenkins suite.


    Great work!  Thanks again

'
---
I began using the the [Jasmine Maven Plugin][1] in June of 2012 and was immediately impressed with how well it worked and how easy it made automating my test execution. Soon after I discovered [require.js][2] and decided to begin using it in my applications. I learned quickly however that the require.js support in the Jasmine Maven Plugin had quite a few issues and so I decided to try and help fix some of them.

Fast-forward to January of this year and I found myself a maintainer of the plugin with full commit access and a huge list of issues (thank you [Justin Searls][3] for the opportunity). I've had a few goals for my first release:

*   don't break anything (still crossing my fingers on this one) 
*   make spec runner templates more useful by providing more variables 
*   merge the require.js specific code into the default code 
*   make the behavior of the `jasmine:bdd` goal and the `jasmine:test` goal consistent 
*   improve overall code quality and setup checks to monitor and measure code quality 

I'm happy to say that version 1.3.1.0 is out and while only time will tell if I didn't break anything and improving code quality is ongoing, I am confident that I achieved my goals. For a full list of bug fixes and enhancements in 1.3.1.0 go [here][4]

Please check out the [new site][5] for information on usage of the plugin and post any [issues you find on github][6].

The [next release][7] is planned for a little over a month from now and will have some new exciting features including support for using [PhantomJS][8] rather than HtmlUnit for headless test execution.

Enjoy!

 [1]: http://searls.github.com/jasmine-maven-plugin
 [2]: http://requirejs.org
 [3]: http://about.me/searls
 [4]: http://searls.github.com/jasmine-maven-plugin/github-report.html
 [5]: http://searls.github.com/jasmine-maven-plugin/
 [6]: https://github.com/searls/jasmine-maven-plugin/issues
 [7]: https://github.com/searls/jasmine-maven-plugin/issues?milestone=2
 [8]: http://phantomjs.org/
