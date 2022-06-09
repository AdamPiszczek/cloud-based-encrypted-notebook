## Authors 😀
- [Kacper Kilianek](https://github.com/Kkilianek)
- [Adam Piszczek](https://github.com/AdamPiszczek)
- [Mateusz Cegielski](https://github.com/MateuszCegielski)

## Website view ⛰️
![Process of creating new note](https://github.com/AdamPiszczek/cloud-based-encrypted-notebook/blob/main/media/website_view.gif)

## Setup 🛠️
- Linux 🐧 / macOS 🍎 version
```sh
> pip install ./requirements.txt
> python3 manage.py makemigrations
> python3 manage.py migrate
> python3 manage.py collectstatic
> python3 manage.py runserver
```
- Windows ☁️ version
```sh
> pip install -r ./requirements.txt
> python manage.py makemigrations
> python manage.py migrate
> python manage.py collectstatic
> python manage.py runserver
```
<ins>Before the first run, ensure that you have on and active PostgreSQL database.</ins>

## How to Run 🏎
- Linux 🐧 / macOS 🍎 version
```sh
> python3 manage.py runserver
```
- Windows ☁️ version
```sh
> python manage.py runserver
```

## Dependiencies 👷 (also attached in ./requirements.txt)
- certifi>=2018.10.15
- chardet>=3.0.4
- Django>=2.1
- django-crispy-forms>=1.7.2
- idna>=2.7
- pytz>=2018.5
- requests>=2.19.1
- urllib3>=1.23
- bcrypt>=3.2.2
- psycopg2==2.9.3
- whitenoise==6.1.0
- django_cryptography>=1.1
- crypto-utils>=1.0.0
- python-dotenv==0.19.0
- django_password_validators>=1.7.0

## Design ℹ️
It is mainly based on the Django framework, and most of its very popular modules are used (mainly components responsible for the security of the application).

## About 📙
The application was created for the safe storage of your notes in a distributed environment. The focus was on the ease and compatibility of the application, so that a given user would be able to log into the website and read / create their next entries at any place and at any time. The very structure of the elements in the back room remains very simple, as these are operations that do not require complex animations or various kinds of fountains. In our case, simplicity and security were left to the client, so that the client could be sure that his secured data would remain encrypted and even breakneck to decrypt. Therefore, the main goal was to solve the risk problems associated with possible attacks from outside. Thanks to the Django framework used, the application was already basically secured with simple elementary operations, which, for example, made it impossible to inject various types of bad SQL queries (SQL injection). More on security and a more extensive description of the tools used can be found in the following chapters of this document.
