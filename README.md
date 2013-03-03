# pathfinder-prd-markdown

A project to convert the pathfinder prd into markdown for the purpose of making
an ebook (or collection of ebooks)

## House Rules
For house rules, such as conventions and submissions, see the wiki.

## How to help!

The easiest way to help is to start editing! If you're familiar with pandoc, to
convert html into markdown, this project uses

    pandoc thing.html --atx-headers --no-wrap -o thing.markdown
    
to start off with. The stripped html is found in the pathfinder folder (not the 
markdown folder) and all markdown files should be placed in the markdown folder. 
All links should be implicit, so compliation requires pandoc 1.10 ish.

If you're not comfortable with actually creating content, beta testing is needed. 
Simply go into the build folders of the markdown folder 
(i.e. markdown/<book of choice>/build) and get the epub. Feedback is welcome on 
dodgy tables (tables that didn't render properly etc.), more logical layout for
an ebook etc. If an issue is found, use github's built in issue tracking system
to report it. IF there are many minor bugs (e.g. missing a space between two 
words) then just file one report with all of the bugs listed.

In the future, the markdown will also be formatted to be 'prettier' but this is a
secondary objective to creating the ebook, so will probably start happening after 
everything is converted from html to markdown to epub.
