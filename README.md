# prd-markdown

## Note: this project is ready to accept submissions!

Subissions of content should follow the guidelines laid out on the wiki. It 
basically boils down to three things:

1. use the pandoc method outlined in this README
2. Implicit links should be used where possible.
3. Word wrap all files to 65 chars 'manually' (I use emacs M-q shortcut).

A project to convert the PF prd into markdown for the purpose of making
an ebook (or collection of ebooks)

## House Rules
For house rules, such as conventions and submissions, see the wiki.

## How to help!

The easiest way to help is to start editing! If you're familiar with pandoc, to
convert html into markdown, in general this project uses

    pandoc thing.html --atx-headers --no-wrap -o thing.markdown
    
to start off with. The stripped html is found in the PF folder (not the 
markdown folder) and all markdown files should be placed in the markdown folder. 
All links should be implicit, so compliation requires pandoc 1.10 ish.

If you're not comfortable with actually creating content, beta testing is needed. 
Simply go into the build folders of the markdown folder 
(i.e. markdown/<book of choice>/build) and get the epub. Feedback is welcome on 
dodgy tables (tables that didn't render properly etc.), more logical layout for
an ebook etc. If an issue is found, use github's built in issue tracking system
to report it. If there are many minor bugs (e.g. missing a space between two 
words) then just file one report with all of the bugs listed (but don't wait 
to report it; someone might get there before you!).

In the future, the markdown will also be formatted to be 'prettier' but this is a
secondary objective to creating the ebook, so will probably start happening after 
everything is converted from html to markdown to epub.

## Legal Stuff

This ebook collection is produced under the Open Game License (OGL). It is also in
compliance with the Community Use Policy (CUP), although no content has *yet* been
taken from the community; This is more of a precautionary measure to ensure that
if the time comes that this project does include community content, everything is
properly covered.

The OGL requires a copy of the OGL in everything released under the license. This 
is included in LICENSE.markdown.

The CUP requires this statement to be on anything that uses the Policy,

> This epub/markdown project uses trademarks and/or copyrights owned by Paizo 
> Publishing, LLC, which are used under Paizo's Community Use Policy. We are
> expressly prohibited from charging you to use or access this content. This 
> epub/markdown project is not published, endorsed, or specifically approved
> by Paizo Publishing. For more information about Paizo's Community Use Policy,
> please visit paizo.com/communityuse. For more information about Paizo Publishing
> and Paizo products, please visit paizo.com.

This statement should always be adhered to in any part of the project. This project
is registered at http://paizo.com/communityuse/registry under the name 'PRD Markdown'
as required by the CUP.
