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

Install the web app::

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
    $ docker run -d -p 5000:5000 flask-blog-application


Wheel 
-------

Install wheel

    $ pip install wheel

Create wheel

    $ python setup.py bdist_wheel
    
On the target machine, install the wheel

    $ pip install dist/flaskr-1.0.0-py3-none-any.whl

Run

    $ flask --app flaskr init-db
    $ flask --app flaskr run --debug

<!-- Test
----

::

    $ pip install '.[test]'
    $ pytest

Run with coverage report::

    $ coverage run -m pytest
    $ coverage report
    $ coverage html  # open htmlcov/index.html in a browser -->
