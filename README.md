# Refactor-Matters
Refactor Code for Marketing Company Unit 1 Homework

# Updating Semantics
This program is to make user friendly existing site via simplifying and organizing.  In particular we are organizing behind the scenes in the coding of both html and css files.

The site has a main header with title and 3 linked inline list times.  Clicking any of the linked items should redirect you lower on the page to the corresponding information section.

You will additionally find a side bar of information pertaining to the purpose of the company and lastly the footer with copyright information

# Link for direct access to both html website and github websites

1. HTML: 

2. GITHUB: 

# Final Image of Website Page

![Screenshot of Finish Website](./assets/images/refactor-is-here-screen.png)

# Find below the history of updates to working file

    ## Update Main Title for the Webpage
        This webpage should be properly titled Horiseon, not "website"

    ## Update the semantics regarding the div for Header in html file
        The html class "header" will be replaced as standard notation. As a result multiple changes to the CSS stylesheet will be updated.  Remove the "." from in front of each "header" class in CSS

    ## H1 Span Option
        The color for the SEO on the Horiseon in h1 is too similar and can barely see it, if we want it to stand out, we need a bolder color choice (gray). Additionally, no need to create a class, recall in css file simply by section name span

    ## Want to ensure all our header links are responsive as expected
        Add the ID for the Search Engine Optimization so that it jumps the page to the expected section

    ## Clean up some div tags in html
        For semantics let's make each major block in the body a section, as opposed to div. The exception is the first div in Body, since it is background, renamed the class "background" for clarity

    ## Footer
        Instead of creating a class footer, let's use the footer tag for the section block

    ## Now Let's Adjust the CSS and Class sets

        If I follow the flow of the html to the stylesheet, I have to move some things around

        ## Benefits section vs the Content section

            Benefits section is placed ahead of contents section in stylesheet so we'll swap that around for now. Also there is a lot of repetition in code in both Content section and Benefits section

        ### Content Section
            Let's concise the coding in the style sheet, this will require removing some classes and defaulting them to the parent section

            Since we have a class for Content  and one for Benefits and all div items and h2/h3  items and img items have the same dimensions, we do not need individual classes for these items, all CSS attributes can be applied through nested classes use the tag names alone under content class and the same for under the benefits class

        ### Benefits Section
            Additionally in the benefits section, since the div had no distinguishable name, to make post coding easier, added individual id labels in the html for the benefits section