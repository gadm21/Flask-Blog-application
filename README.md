# Flask-Blog-application


A basic blog application written in Flask.

Install
-------

    # clone the repository
    $ git clone https://github.com/gadm21/Flask-Blog-application
    $ cd Flask-Blog-application
    
Create a virtualenv and activate it::

    $ python3 -m venv venv
    $ . venv/bin/activate

Or on Windows cmd::

    $ py -3 -m venv venv
    $ venv\Scripts\activate.bat

Install Flaskr::

    $ pip install -e .
    


Run
---


    $ flask --app flaskr init-db
    $ flask --app flaskr run --debug

Open http://127.0.0.1:5000 in a browser.


Docker 
-------

Install Docker 

    $ sudo snap install docker

Build and run

    $ docker build -t flask-blog-application .
    $ docker run flask-blog-application

<!-- Test
----

::

    $ pip install '.[test]'
    $ pytest

Run with coverage report::

    $ coverage run -m pytest
    $ coverage report
    $ coverage html  # open htmlcov/index.html in a browser -->
