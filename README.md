<div align="center">
  <img src="LISP_logo_mid.png">
</div>

# Awesome Common Lisp Learning List [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

This list focuses on resources for learning Common Lisp, especially resources that I've found useful.

There are other awesome Common Lisp lists that focus on other topics:
* [Awesome Common Lisp Libraries](https://github.com/CodyReichert/awesome-cl)
* [Curated Awesome Common Lisp Libraries](https://github.com/vindarel/curated-awesome-cl) (forked and updated from the above list)
* [Awesome Common Lisp Software](https://github.com/azzamsa/awesome-cl-software)

Contributions are welcome. Please submit a pull request or create an issue to add to the list.

## How To Use
1. Get a Lisp environment.
2. Bookmark the [The Common Lisp Hyperspec](http://www.lispworks.com/documentation/common-lisp.html).
3. Download and work through a Lisp book of an appropriate level. Type the examples and play with the code. Feel free to switch books and try a different one.
4. Try out [Exercism](http://exercism.io/languages/common-lisp/about).
5. [Ask smart questions](http://www.catb.org/esr/faqs/smart-questions.html) in an online community if you get really stuck.
6. Learn about [Quicklisp](https://www.quicklisp.org/beta/).
7. At some point, read your Lisp implementation's manual.

## Lisp Environments
You can run a Lisp implementation directly, but an editing environment makes the experience easier.
* Prepackaged environments
  * [Portacle](https://shinmera.github.io/portacle/), a portable and multiplatform Common Lisp environment. It ships a slightly customized Emacs with SLIME, SBCL (a popular Common Lisp implementation), Quicklisp and Git. No installation needed, so it's a very quick and easy way to get going.
  * [Lispbox](https://common-lisp.net/project/lispbox/), an IDE (Emacs + SLIME), Common Lisp implementation (Clozure Common Lisp) and library manager (Quicklisp), pre-packaged as archives for Windows, Mac OSX and Linux. Descendant of "Lisp in a Box" [mentioned](http://www.gigamonkeys.com/book/lather-rinse-repeat-a-tour-of-the-repl.html) in Practical Common Lisp.
  * [Lispworks Personal Edition](http://www.lispworks.com/downloads/) is a non-Emacs based IDE for LispWorks Lisp, with some restrictions.
  * [Allegro Common Lisp](https://franz.com/products/allegrocl/) has a free [Express Edition](https://franz.com/downloads/clp/survey) IDE, and [training videos on Youtube](https://www.youtube.com/channel/UCN36UrxtyNBJPaG0kmBJNRw).
* For advanced users
  * [Articulate Common Lisp](http://articulate-lisp.com/) is a HOWTO for putting together a Lisp environment, and has information on [useful libraries](http://articulate-lisp.com/project/abcs.html) and how to [structure projects](http://articulate-lisp.com/project/new-project.html).
  * If you're an experienced [Emacs](https://www.gnu.org/software/emacs/) user, you can just install [SLIME](https://common-lisp.net/project/slime/) and a [supported Common Lisp implementation](https://common-lisp.net/project/slime/doc/html/Platforms.html#Platforms). See the [SLIME manual](https://common-lisp.net/project/slime/doc/html/) for more details.
  * The Common Lisp Cookbook has more information about [installing an implementation](https://lispcookbook.github.io/cl-cookbook/getting-started.html) using an implementation manager like [Roswell](https://github.com/roswell/roswell/wiki), or on Docker.

## Online References
* [The Common Lisp Hyperspec](http://www.lispworks.com/documentation/common-lisp.html) (CLHS) is _the_ language reference document for Common Lisp. Bookmark it now.
* [The Common Lisp Cookbook](http://lispcookbook.github.io/cl-cookbook/) is a list of useful Lisp recipes. Also contains a list of other online sources of CL information.
* [Common Lisp, the Language by Guy L. Steele](https://www.cs.cmu.edu/Groups/AI/html/cltl/cltl2.html) is a description of the Common Lisp language from just before it was standardized by ANSI. Some parts are outdated, but it contains better descriptions of [LOOP](http://www.cs.cmu.edu/afs/cs.cmu.edu/project/ai-repository/ai/html/cltl/clm/node235.html#SECTION003000000000000000000) and [FORMAT](http://www.cs.cmu.edu/afs/cs.cmu.edu/project/ai-repository/ai/html/cltl/clm/node200.html) than the CLHS does.

## Online Books
These books that are freely accessible online, arranged roughly in order from basic to advanced:
* [Common Lisp: A Gentle Introduction to Symbolic Computation by David S. Touretzky](http://www.cs.cmu.edu/~dst/LispBook/) is a good introduction for people new to programming. Contains code for really useful utilities like [DTRACE](http://www.cs.cmu.edu/~dst/Lisp/dtrace/) and [SDRAW](http://www.cs.cmu.edu/~dst/Lisp/sdraw/).
* [Practical Common Lisp by Peter Seibel](http://www.gigamonkeys.com/book/) is a great introduction for experienced programmers, and tries to highlight from the very beginning what makes CL different to other languages.
* [Common Lisp: An interactive approach by Stuart C. Shapiro](https://www.cse.buffalo.edu/~shapiro/Commonlisp/) is a textbook that teaches mainly through the use of exercises.
* [On Lisp by Paul Graham](http://www.paulgraham.com/onlisp.html) is a great book for intermediately experienced Lispers.
* [Paradigms of Artificial Intelligence Programming by Peter Norvig](https://github.com/norvig/paip-lisp) is another classic book.
* [Let Over Lambda by Doug Hoyte](https://letoverlambda.com/) is an advanced book on Lisp Macros. [Several people recommend](https://www.reddit.com/r/lisp/comments/3actsc/let_over_lambda/) that you be comfortable with On Lisp before reading this book, and that the start is slow. The first six chapters are available online.

## Offline Books
These are books that you'll have to buy, or borrow from a library.
* [Land of Lisp by Conrad Barski, MD](http://landoflisp.com/) is a fantastically fun introduction to Lisp that uses comics and has you writing games.
  * Available as an [ebook](https://www.nostarch.com/lisp.htm).
  * The Web server example in Ch 13 will only work on CLISP.
  * A couple of the LOOP macros are written `for x for y...` which you can change to `for x from 0 for y...` to make them work in SBCL.
  * Has an [errata page](http://landoflisp.com/errata.html).
* [ANSI Common Lisp by Paul Graham](http://www.paulgraham.com/acl.html) is good as a reference, covers CLOS, and has several example program implementations.
* [Common Lisp Recipes by Edmund Weitz](http://weitz.de/cl-recipes/) is a great set of Common Lisp patterns.
* [Lisp in Small Pieces](https://pages.lip6.fr/Christian.Queinnec/WWW/LiSP.html), is an _"excellent book on Lisp implementation. You'll get a lot out of it, whether you are interested in writing compilers and interpreters (for Lisp or any language) or whether you just want to see how Lisp works."_ - Peter Norvig's review on the [Amazon product page](https://www.amazon.com/Lisp-Small-Pieces-Christian-Queinnec/dp/0521545668/).

<!-- Adam Tornhill's AMOP sequence (PCL -> OOP in CL -> AMOP): http://www.adamtornhill.com/reviews/amop.htm  -->

## Online Community
* The [Cliki](http://cliki.net) is the Common Lisp Wiki. A great resource for all things CL. Has a great [Getting Started](http://cliki.net/Getting+Started) page and an extensive list of [Lisp books](http://cliki.net/Lisp%20books).
* The #clnoobs room on the [Freenode IRC network](http://freenode.net/) is active and friendly.
* The [Lisp Subreddit](http://www.reddit.com/r/lisp/) is an active community, and has loads of useful links and reference documents in the sidebar.
* [Exercism's Common Lisp track](http://exercism.io/languages/common-lisp/about) is an excellent way to learn the language through practice, have your code reviewed, and to discuss solutions with other people.
* The [Lisp Discord server](https://discord.gg/GEyD6) has a channel dedicated to Common Lisp and will happily answer questions.

## Libraries
These aren't libraries, but can help you find and install other libraries.
* [Quicklisp](https://www.quicklisp.org/beta/), a package management platform for Lisp libraries.
* [Quickdocs](http://quickdocs.org/), documentation for projects in Quicklisp
* [State of the Common Lisp Ecosystem, 2015](http://borretti.me/article/common-lisp-sotu-2015) talks about what libraries you should use, and why.
* The Articulate Common Lisp site [lists some useful libraries](http://articulate-lisp.com/project/abcs.html).
* As mentioned at the top, the [Awesome Common Lisp](https://github.com/CodyReichert/awesome-cl) and [Curated Awesome Common Lisp](https://github.com/vindarel/curated-awesome-cl) lists focus on libraries.


## Common Lisp Implementation
This section lists some common CL implementations and their manuals in alphabetical order. Unless otherwise noted, these are free software implementations. See also the Cliki's list of [free software Common Lisp Implementations](https://www.cliki.net/Common%20Lisp%20implementation).
* [Allegro Common Lisp](https://franz.com/products/allegrocl/) (ACL) and [manual](https://franz.com/support/documentation/). Commercial, but has a free [Express Edition](https://franz.com/downloads/clp/survey) and [training videos on Youtube](https://www.youtube.com/channel/UCN36UrxtyNBJPaG0kmBJNRw).
* [CLISP](https://clisp.sourceforge.io/) and [manual](https://clisp.sourceforge.io/impnotes.html).
* [Clozure](https://ccl.clozure.com/) Common Lisp (CCL) and [manual](https://ccl.clozure.com/manual/).
* [Carnegie Mellon University Common Lisp](https://www.cons.org/cmucl/) (CMUCL), has a [manual and other useful information](https://www.cons.org/cmucl/doc/index.html).
* [Embeddable Common Lisp](https://common-lisp.net/project/ecl/) (ECL) and [manual](https://common-lisp.net/project/ecl/static/manual/).
* [LispWorks](http://www.lispworks.com/products/index.html) and [manual](http://www.lispworks.com/documentation/index.html). Commercial, but as mentioned previously, has a [Personal Edition](http://www.lispworks.com/downloads/index.html) with minor limitations.
* [Steel Bank Common Lisp](http://www.sbcl.org/) (SBCL) and [manual](http://www.sbcl.org/manual/index.html). My personal favorite.
* [Scieneer Common Lisp](http://www.scieneer.com/scl/) (SCL) and [manual](http://www.scieneer.com/scl/doc/). A commercial Linux and Unix implementation, but has an unrestricted free evaluation and non-commercial use version.

## Credit
I got a lot of the information from [Rainer Joswig's StackOverflow answer on learning Common Lisp](https://stackoverflow.com/a/7224914/1005039), and from the now-defunct StackOverflow Documents site. The [Cliki's Getting Started](https://cliki.net/Getting%20Started) page was also invaluable.

## License
[![Creative Commons License](http://i.creativecommons.org/l/by/4.0/88x31.png)](https://creativecommons.org/licenses/by/4.0/)

This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).
