# Guide to Modifying the HIPERFIT Web Site

## Introduction

The HIPERFIT web site is based on
[Jekyll-Bootstrap](http://jekyllbootstrap.com), which again is based
on [Twitter Bootstrap](http://twitter.github.com/bootstrap/), Jekyll,
and Liquid. Bootstrap gives a standard set of CSS/Javascript tools and
Jekyll gives us markdown support and a (very limiting) template system
based on Liquid.

The site is hosted at github as <http://hiperfit.github.com>. We use
the <http://hiperfit.dk> domain for the site, which has been enabled
by directing the domain to the github IP and by placing a file CNAME
(containing hiperfit.dk) in the root.

## Modifying Web Site Content

To modify the Web Site content, one needs a github account name and
authorization to push changes to the hiperfit.github.com repository.

Github has Jekyll and Liquid built-in, which means that once a changed
is pushed to github, the site is rebuilt on github.

## Structure

Images are stored into the `images/` folder and papers (pdfs, etc)
are stored into the `pdf/` folder.

## Creating New Posts

Posts are stored in the `_posts` folder. For creating a new post you
can either run the command

   rake post title="My Title" date="YYYY-MM-DD"

which will create an empty post file, or you can copy one of the
existing post files - be sure to format the post file name correctly.

## Creating New Pages

Pages can be stored in any folder (without a prefix underscore). For
creating a new page you can either run the command

   rake page title="My Title"

which will create an empty page file, or you can copy one of the
existing pages. For inspiration on the markdown syntax, look at one of
the existing .md-files.


