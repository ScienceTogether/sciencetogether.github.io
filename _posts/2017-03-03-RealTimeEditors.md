---
layout: post
title:  "Real Time editors"
date:   2017-03-03 12:00:59 +0100
authors: 
  - DavidPS
  - danielStrien
  - tcouch
  - Patricia
  - danb
  - fedago
categories: unconference editors 1session
---


![discussion on real time editors](/assets/realtime_editors.jpg){:class="img-responsive"}

## What are our requirements?

 - Browser based (many people cannot install things at their work computers)
 - Edit offline option (not everytime we've got access to internet)
 - Anonymous access (so collaborators no need to create an account)
 - Integration with a reference management.
 - LaTeX
 - Git backend
 - Export to MS word?
 - Track changes
 
 
## Problems and solutions to our requirements
 
 - If anonymous access, how do we know who wrote that? Etherpad allows you to
   identify yourself with a pseudonym. That is quite useful.
 - LaTeX is not easy understood by everyone, but tools
   like [DropboxPapers](https://paper.dropbox.com/) allows to insert blocks with
   it. Also LaTeX editors
   like
   [Authorea](https://www.authorea.com/), [Overleaf](https://www.overleaf.com/),
   ... lets you edit in rich text mode.
 - Offline mode like offered by google drive on mobile devices or through git
   backend like Overleaf, however is not clear how the possible "conflicts" are
   managed. Needed to test.
 - Reference managers are offered by some editors,
   however [zotero](https://www.zotero.org/) allows you to drag and drop from
   the collection via the
   [quick copy](https://www.zotero.org/support/creating_bibliographies#quick_copy) 
   feature and you can put the reference anywhere you like.
 - Export to MS word can we done from various commands using [pandoc](http://pandoc.org/),
   though not perfect it's quite good.
 - Tracking changes is offered by many editors, some betters than others though.
 
## The MS Word nightmare

We all have suffered at least once this nightmare. You are writing a document
and sharing with people by e-mail, then each of the collaborators uses their way
to contribute. For example:
 - Send you (only you) an email with text like:
 ```
 * In line 10 change color by colour.
 * Paragraph 3 doesn't make sense, this could be better:
   "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam consequat,
 erat quis iaculis sagittis, orci enim volutpat velit,..." 
 * I don't believe the fifth word in the second paragraph on the  eleventh page 
   makes sense. We need to discuss it.
 ```
 - Reply to all with a new version of the document, without tracking changes activated.
 - Idem, but with a new file name with name and date: `thisreport.Ramon.29Dec2017.doc`
 - Reply with comments in the document where the comments are not comments but
   editions to the document.
 - Iterations of all the above once and again, replicating files everywhere.
 
 We discussed the ways to solve this type of situations. The reasons of why
 people do this things could be to do with many factors, from respect to don't 
 correct someone else's text to be scared to break the files.
 
 We believe the following may help to solve this problems.
 
 1. Use a collaborative interface when possible (Google docs, Overleaf, ...)
 1. Clearly state the workflow to follow *e.g.*: use reply all, suggesting or
    track changes mode, 
 1. Name a person as the editor of the document.
 
## Conclusions of the session

We put under test few tools and update
[the info on the tools description](https://github.com/ScienceTogether/tools/commit/59d55e93bba5a50ff948363680b28397e78ce288).
We found that some tools we really liked were not fulfilling our needs as
we thought, and others were not as simple as we thought they were.
 
Finally we crown the Google docs suite as it's similar enough to MS word, you
can edit a document anonymously (only with a link) and it allows different
setting like suggesting new text, commenting and browsing history.
We crown Overleaf when we can teach or works with others using LaTeX as it offers
similar features and it's backed up using git.
