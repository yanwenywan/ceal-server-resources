# Useful Tips

A collection of some useful tips and tidbits about writing mkdoc markdown for this project.

## Attribute Lists

[Attribute lists](https://python-markdown.github.io/extensions/attr_list/) allow you to add custom HTML formatting to elements (such as images) inline in markdown, which is not supported by default. They come in the form

    {: #someid .someclass somekey='some value' }

One use of them is to scale images, e.g. by doing the following:

    ![](img/fuller1.png){: style="height: 400px"}

This sets the image `fuller1.png` to a height of 400 pixels. 

Knowledge of HTML and CSS is required.  
