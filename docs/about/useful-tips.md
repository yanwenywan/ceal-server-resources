# Useful Tips

A collection of some useful tips and tidbits about writing mkdoc markdown for this project.

## Attribute Lists

[Attribute lists](https://python-markdown.github.io/extensions/attr_list/) allow you to add custom HTML formatting to elements (such as images) inline in markdown, which is not supported by default. They come in the form

    {: #someid .someclass somekey='some value' }

One use of them is to scale images, e.g. by doing the following:

    ![](img/fuller1.png){: style="height: 400px"}

This sets the image `fuller1.png` to a height of 400 pixels. 

Knowledge of HTML and CSS is required.  

## Frontmatter

Frontmatter is a special section in a markdown document that appears at the **top** of the page. It is **optional**. It contains extra attributes about the page that is used by some other plugins. You write it between two `---` triple dash lines like so (the first and last lines show file boundaries only):

    ==============tangut.md================
    ---
    title: Tangut
    description: A basic primer on how to read Tangut
    ---

    Blah blah blah blah...
    =======================================

The frontmatter is a **yaml format**, same as `mkdocs.yml`. Below are some attributes that you can write:

- `title: ...` Changes the name of the tab on the browser bar. This defaults to the page title from the `#` header or whatever you set in `nav`, so *generally you don't need to touch this*.
- `description: ...` Gives the page its own description. This is used primarily to populate the "social cards" -- fancy previews that you see when a link is pasted into somewhere like discord. If you don't put anything here, it will use the default website description. (see below)
    
    ![Description in social card](img/preview.png){: style="max-width: 300px;"}

