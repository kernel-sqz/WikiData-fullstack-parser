# Appsilon Homework

![empty_db](https://github.com/kernel-sqz/appsilon-homework/blob/main/img/Zrzut%20ekranu%202023-05-2%20o%2023.12.22.png | width=100)
![table](https://github.com/kernel-sqz/appsilon-homework/blob/main/img/Zrzut%20ekranu%202023-05-2%20o%2022.08.43.png | width=100)
![description](https://github.com/kernel-sqz/appsilon-homework/blob/main/img/Zrzut%20ekranu%202023-05-2%20o%2022.08.31.png | width=100)

# Description

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

# Backend (django)

> > > $ pip install -r requirements.txt
> > > $ python manage.py runserver

# Frontend (react)

> > > $ npm i
> > > $ npm start
