.. _command-line:

Command line
============

This page provides a syllabus for getting up-to-speed on being
productive on the command line.

If you're planning on running bioinformatics tools or Biowulf, you will need to
get good at using the command line. Even if you're only planning on using R or
Python, basic command-line usage (at least moving around and listing files)
will be useful.


Optional textbooks
------------------

The resources below are all web-based. Sometimes it’s nice to have a hard-copy
book, so here are some good options:

- `Practical Computing for Biologists
  <https://www.amazon.com/gp/product/0878933913>`_ is a fantastic textbook,
  available on Amazon

- `A Primer for Computational Biology
  <https://open.oregonstate.education/computationalbiology/>`_
  is free and has sections on command-line, Python, and R. You can buy a hard
  copy on `Amazon
  <https://www.amazon.com/Primer-Computational-Biology-Shawn-ONeil/dp/0870719262>`_.

Command line
------------

Most command-line tutorials teach the same sorts of things but in
different ways. You may find some tutorials fit your brain better than
others, so I’ve provided several here. The different tutorials
prioritize different topics, and each has its own unique content. I’ve
tried to indicate this in the descriptions below. One approach you could take
would be to pick one and go through it start-to-finish, and then read through
the remaining tutorials relatively quickly to see if they offer any other
insight or additional information not covered by the others. The benefit of
this approach is that you will also get a review of the topics you’ve already
learned. Another approach could be to take a single topic at a time, and work
through that topic in each of the resources to get practice and see it
presented in different ways.

Here is a list of skills you should have for basic command-line usage:

- open a terminal on your computer
- connect to a remote machine with SSH
- navigate with ``ls``, ``cd``, ``pwd``.
- inspect files with ``head``, ``less``, ``tail``, ``wc``
- search for text in a file with ``grep``
- manipulate delimited text with ``awk``
- sort files with ``sort``
- edit a file with ``nano`` or ``vim`` or ``emacs``
- extract columns with ``cut``
- pipe commands together
- change permissions with ``chmod``
- move, copy, rename files
- make directories
- know the difference between stdin/stdout/stderr
- redirecting stdout and/or stderr
- download files with ``wget`` and/or ``curl``
- creating scripts
- making symlinks -- both to files and directories and how they behave
  differently
- “install” a program by putting it on the ``$PATH``

The resources below will teach you these.

Resources for learning the command line
---------------------------------------

Each of these is partly redundant with the others. Based on feedback
from others going through these resources, the Unix Workbench is more
streamlined and allows you to spend more time on the exercises.

The Unix Workbench
~~~~~~~~~~~~~~~~~~

https://seankross.com/the-unix-workbench

This is the companion text to the Coursera course
https://www.coursera.org/learn/unix. The text is pretty straightforward,
and unlike some other tutorials it includes sections on Bash programming
and Git/GitHub.

A Primer for Computational Biology
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

https://open.oregonstate.education/computationalbiology/

For command-line, all of Part I is fantastic. In addition to the basics, this
book has a section specifically on installing bioinformatics software and
running command-line BLAST. It also has quite a few exercises to work on. Part
II of the book is on Python, Part III is on R. If you are planning on learning
Python or R, reading this book cover-to-cover will get you quite far!

Learn the Command Line
~~~~~~~~~~~~~~~~~~~~~~

https://www.codecademy.com/learn/learn-the-command-line

Like many of the Codecademy tutorials, this is kind of gamified. This can be
a powerful motivator for some people. They want you to sign in, and they offer
paid upgrades.

Learn Enough Command Line to be Dangerous
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

https://www.learnenough.com/command-line-tutorial

This one has some asides to get you up to speed on “programming culture” things
that you will see throughout your career in many contexts, like using ``foo``
or ``bar`` as variable names, or explaining some in-jokes. It’s heavy-handed on
the outdated memes, but if you can get past that it’s pretty good.

.. note::

    For anything beyond chapters 1 and 2, this has recently become a paid
    option -- as of Nov 30 2019 it's $9 for the full content.

Intermediate command line
-------------------------

Here are skills that might be considered more intermediate:

- for loops
- if/else statements
- associative arrays (Bash 5)
- POSIX compliance
- various tests like ``-z``, ``-e``, etc
- subshells
- process substitution
- interpolating command output (with ``$()`` or backticks)
- piping to ``xargs``
- functions
- heredocs
- exit codes
- ``set -x``
- command substitution
- ``set -eou pipefail`` (what it means and why you would want to use it)
- ``[`` vs ``[[``
- ``&&`` vs ``||``

Other intermediate resources:

- Try the `command line challenge <https://cmdchallenge.com/>`_. This gives you
  a series of challenges that you complete directly in the browser and that are
  checked immediately in real time.

- There are many opinions on formatting shell scripts, but the `bash style
  guide <https://google.github.io/styleguide/shellguide.html>`_ used at Google
  seems to have well-thought-out suggestions.

- `bash cheat sheet <https://bertvv.github.io/cheat-sheets/Bash.html>`_ has
  a concise overview of good ways to use bash. This could be thought of as sort
  of an extension beyond the above style guide.

- `Intermediate guide to bash scripting
  <https://www.linode.com/docs/development/bash/an-intermediate-guide-to-bash-scripting/>`_,
  which talks about making menus, printf, and various test options for files and
  directories.

- Julia Evans' `bash quirks <https://jvns.ca/blog/2017/03/26/bash-quirks/>`_
  has some overlap with the previous links and some new ones as well.

- This 3-part blog series starts with why you would want to learn ``awk``
  anyway, and then shows you the ropes. The later tutorials get a bit advanced
  to the point where I would probably be using R or Python instead, but it can
  be useful to know how to do these kinds of things directly from the command
  line.

  - `Why Learn AWK? <https://blog.jpalardy.com/posts/why-learn-awk/>`_
  - `Awk tutorial part 1 <https://blog.jpalardy.com/posts/awk-tutorial-part-1/>`_
  - `Awk tutorial part 2 <https://blog.jpalardy.com/posts/awk-tutorial-part-2/>`_
  - `Awk tutorial part 3 <https://blog.jpalardy.com/posts/awk-tutorial-part-3/>`_
  - `Awk tricks <https://blog.jpalardy.com/posts/my-best-awk-tricks/>`_

- `Defensive bash programming
  <https://kfirlavi.herokuapp.com/blog/2012/11/14/defensive-bash-programming/>`_
  also reiterates some of the suggestions from above and adds some additional ones.

Advanced command line
---------------------

The Linux documentation project's `advanced bash scripting guide
<https://tldp.org/LDP/abs/html/index.html>`_ will keep you busy for a while....
