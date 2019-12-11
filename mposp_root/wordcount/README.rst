=====
Wordcount
=====

Wordcount is a simple Django app to conduct Web-based wordcount. For each
question, visitors can choose between a fixed number of answers.

Detailed documentation is in the "docs" directory.

Quick start
-----------

Download the code from github: 

1. Add "wordcount" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'wordcount',
    ]

2. Include the wordcount URLconf in your project urls.py like this::

    path('wordcount/', include('wordcount.urls')),

3. Run `python manage.py migrate` to create the wordcount models.

4. Start the development server and visit http://127.0.0.1:8000/admin/
   to create a wordcount (you'll need the Admin app enabled).

5. Visit http://127.0.0.1:8000/wordcount/ to participate in the poll.