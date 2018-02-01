.. include:: replace.txt
.. heading hierarchy:
   ------------- Chapter
   ************* Section (#.#)
   ============= Subsection (#.#.#)
   ############# Paragraph (no number)

Submitting new models
---------------------

We actively encourage submission of new features to ns-3. 
Independent submissions are essential for open source projects, and you 
will also be credited as an author of future versions of ns-3. However, 
please keep in mind that there is already a large burden on the ns-3 
maintainers to manage the flow of incoming contributions and maintain new 
and existing code. The goal of this document is thus to outline how you 
can help to minimize this burden and thus minimize the average time-to-merge 
of your code. Making sure that each code submission fulfills as many items 
as possible in the following checklist is the best way to ensure quick 
merging of your code.

In brief, we can summarize the guidelines as follows:

1.  Understand what a code review really is
2.  Be licensed appropriately
3.  Follow the ns-3 coding style and engineering guidelines
4.  Write associated documentation, tests, examples
5.  Prepare carefully your submission
6.  Pick a submission tool

If you do not have the time to follow through the process to include your 
code in the main tree, please see out of tree about contributing ns-3 code 
that is not maintained in the main tree.

Upstreaming new models
**********************
The term ``upstreaming`` refers to the process whereby new code is 
contributed back to an upstream source (the main open source project)
whereby that project takes responsibility for further enhancement and
maintenance.

For instance, if one were to develop a new routing protocol, a new
Wi-Fi rate control, a new device model, etc. and wanted to insert it
into the main ns-3 distribution, one would follow the process outlined here:
https://www.nsnam.org/developers/contributing-code/
namely:

1. Understand what a code review really is and how it will work
2. Be licensed appropriately
3. Follow the ns-3 coding style and engineering guidelines
4. Write associated documentation, tests, examples
5. Prepare carefully your submission
6. Pick a submission tool

The process can take a long time when submissions are large or when
contributors skip some of these steps.  Therefore, best results are found 
when the following guidelines are followed:

* Ask for review of small chunks of code, rather than large patches.  Split
  large submissions into several more manageable pieces.
* Make sure that the code follows the above guidelines (coding style,
  documentation, tests, examples) or you may be quickly asked to fix these
  things before people look at it again.

Externally maintained models
****************************
Some projects choose to maintain their own version of ns-3, or maintain models
outside of the main tree of the code.  In this case, the way to find out
about these is to look at the Related Projects page on the wiki:
https://www.nsnam.org/wiki/Related_Projects

If you know of externally maintained code that the project does not know about,
please email ``webmaster@nsnam.org`` to request that it be added to the
list of external projects.

Unmaintained, contributed code
******************************

Anyone who wants to provide access to code that has been developed to 
extend ns-3, but who chooses not to go through the above review process, 
may list its availability on our website. Furthermore, we will provide 
storage on a web server if needed. This type of code contribution will 
not be formally maintained by the project, although popular extensions 
might be adopted downstream.

We ask anyone who wishes to do this to provide at least this information 
on our wiki:

* Authors,
* Name and description of the extension,
* How it is distributed (as a patch or full tarball),
* Location,
* Status (how it is maintained)

The contribution will be stored on our wiki at 
https://www.nsnam.org/wiki/index.php/Contributed_Code
here. If you need web server 
space for your extension, please contact one of the project maintainers.

