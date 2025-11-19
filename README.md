# [東方古文學會藏書館 CEAL Server Resources](https://ceal.yanwenyuan.uk)

Guides, Papers, books, and other useful resources for Classical Chinese or Classical East Asian languages in general, contributed by members of the _Classical East Asian Languages_ discord server.

-----

### Running Locally 

This website is written using [MkDocs](https://www.mkdocs.org/) with the `mkdocs-material` theme.

#### Instructions

This workflow has been tested on **Python 3.13** on an Arch-based linux system. However it should work everywhere just as well as long as you have python.

1. Create a virtual environment for mkdocs (or use your global one if you're masochistic)    
    `python -m venv venv`
2. Activate that environment in a terminal    
    `source venv/bin/activate`    
    (note: on windows you have to run the bat file)
3. `pip install -r requirements.txt`
4. run `mkdocs serve` to get the live server. In a browser you can go to `localhost:8000`, and it should auto-update as you write.

