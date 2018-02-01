.. include:: replace.txt
.. heading hierarchy:
   ------------- Chapter
   ************* Section (#.#)
   ============= Subsection (#.#.#)
   ############# Paragraph (no number)

General
-------

This section pertains to general topics about licensing, coding style,
and tools to create patches and code for submission.

Licensing
*********
All code submitted must be GNU GPLv2 compatible.  Please see 
https://www.nsnam.org/developers/contributing-code/licensing/
for more information.

Copyright
*********
The project does not maintain copyright of contributed code; it remains
with the author(s) or their employer.  Please consult with your organization
if you are unsure about which copyright to list for newly contributed code.

When originating a new file, the originating author should place his or her
copyright statement at the top in the header, preceding the copy of the
license.  An important exception to this is if the new file is copied from
somewhere else and modified to make the new file; please do not delete
the previous copyrights from the copyright file!  In such a case, you may
add your copyright to the previous list of copyrights.

Attribution
***********
We ask that contributors refrain from aggressively inserting statements
of attribution into the code such as:

::

  // New Hello Timer implementation contributed by John Doe, 2014

because, over time, it clutters the code.  The mercurial tool is used
to track who contributed what over time.

Likewise, if someone contributes a minor enhancement or a bug fix to
an existing file, this is not typically justification to insert an
``Authored by`` or ``Copyright`` statement at the top of the file.  If
everyone who touched a file did this, we would end up with unwieldy
lists of authors on many files.  In general, we recommend to follow
these guidelines:

* if you are authoring a new file or contributing a substantial portion
  of code (such as 30% or more new or changed statements), you can
  list yourself as co-author or add a new copyright to the file header
* if you are modifying less than the above, please refrain from adding
  copyright or author statements as part of your patch
* do not put your name or your organization's name anywhere in the
  main body of the code, for attribution purposes

Coding style
************
We ask that all contributors make their code conform to the 
coding standard which is outlined here:
https://www.nsnam.org/developers/contributing-code/coding-style/

The project maintains a Python program called ``check-style.py`` found in
the ``utils/`` directory.  This is a wrapper around the ``uncrustify``
utility with configuration set to the conventions used by |ns3|.

Creating a patch
****************
Patches can be attached to a bug report or sent to the mailing-lists.

The UNIX diff tool is the most common way of producing a patch: a patch is 
a text-based representation of the difference between two text files or two 
directories with text files in them. If you have two files, 
``original.cc``, and, ``modified.cc``, you can generate a patch with the 
command ``diff -u original.cc modified.cc``. If you wish to produce a patch 
between two directories, use the command ``diff -uprN original modified``.

Make sure you specify to the reviewer where the original files came from 
and make sure that the resulting patch file does not contain unexpected 
content by performing a final inspection of the patch file yourself.

Patches such as this are sufficient for simple bug fixes or very simple 
small features.

When using mercurial, the mercurial tool can be used to create a patch
of what parts differ from the last committed code; see 
http://selenic.com/hg/help/diff

Rietveld
********
The project uses a code review tool known as Rietveld, developed by
Guido van Rossum.  It is hosted on the Google App Engine, and requires 
a Gmail account for contributors to leave comments.  Examples of code
reviews for ns-3 are found at
https://www.nsnam.org/wiki/Current_Development#Code_reviews

Please see the following web resources for more information:
* https://www.nsnam.org/developers/tools/rietveld/
* https://www.nsnam.org/wiki/index.php/HOWTO_control_Rietveld_patch_generation

Maintainers
***********
Maintainers are the set of people who make decisions on code and documentation
changes.  Maintainers are those people who have demonstrated, over time,
knowledge and good judgment as pertains to contributions to |ns3|, and who
have expressed willingness to maintain some code.  |ns3| is like other 
open source projects in terms of how people gradually become maintainers
as their involvement with the project deepens; maintainers are not newcomers
to the project.

The list of maintainers is found here:
https://www.nsnam.org/developers/maintainers/

Maintainers review code (bug fixes, new models) within scope of their 
maintenance responsibility.  A maintainer of a module should "sign off"
(or approve of) changes to an ns-3 module before it is committed to
the main codebase. 

Note that some modules do not have active maintainers; these types of 
modules typically receive less maintenance attention than those with
active maintainers (and bugs may linger unattended).

The best way to become a maintainer is to start by submitting patches
that fix open bugs or otherwise improve some part of the simulator.
People who submit quality patches will catch the attention of the maintainers
and may be asked to become one at some future date.

People who ask to upstream a new module or model so that it is part of the
main ns-3 distribution will typically be asked to maintain it going forward
(or to find new maintainers for it).

Consortium
**********
The NS-3 Consortium is a collection of organizations cooperating to 
sustain the ns-3 project.  It operates in support of the open source project 
by providing a point of contact between industrial members and ns-3 
developers, by sponsoring events in support of ns-3 such as users' days and 
the annual Workshop on ns-3, by guaranteeing maintenance support for 
ns-3's core, and by supporting administrative activities necessary to 
conduct a large open source project.

Membership to the Consortium is open to those institutions that sign the 
membership agreement and agree to pay an annual recurring membership fee.
The Consortium is overseen by a Steering Committee composed of individuals 
appointed by Executive Members of the Consortium.  More information can
be found at the following URL:  https://www.nsnam.org/consortium/about/

