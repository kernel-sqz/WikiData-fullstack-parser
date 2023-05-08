# WikiData fullstack parser

![empty_db](https://github.com/kernel-sqz/appsilon-homework/blob/main/img/Zrzut%20ekranu%202023-05-2%20o%2023.12.22.png)
![table](https://github.com/kernel-sqz/appsilon-homework/blob/main/img/Zrzut%20ekranu%202023-05-2%20o%2022.08.43.png)
![description](https://github.com/kernel-sqz/appsilon-homework/blob/main/img/Zrzut%20ekranu%202023-05-2%20o%2022.08.31.png)

# Description
The main goal is to search for every movie made after 2013, add it to data base and display in table using React-Table.
- Backend endpoints:

  - /api/movies/

  - Query parameters:

        ?title - (e.g. ?title=s) Will return every movies that title starts with 's'
        ?update (boolean) - When update parameter is set to 'true' script will check for updates from 'https://query.wikidata.org'
        ?page (number) - Go to page (number)
        ?page_size (number) - Return (number - default 10) objects

Example of saved movie in database:

    {
      "movie": "http://www.wikidata.org/entity/Q18407",
      "imdb_id": "tt0053779",
      "title": "La Dolce Vita",
      "date": "2020-03-20"
    }

# How to run it?

## Backend (django)
Go to directory that contains backend files and execute those commands:

    $ pip install -r requirements.txt
    $ python manage.py runserver

## Backend (django) with virtual enviroment
Go to directory that contains backend files and execute those commands:

`*`3.xx = your python version. Recomended 3.11

    $ virtualenv venv -p python3.xx
    $ source ./venv/bin/activate
    $ pip install -r requirements.txt
    $ python manage.py runserver

## Frontend (react)
Go to directory that contains frontend files and execute those commands:


    $ npm i
    $ npm start
