# Project Elixir

* Nicole Barucha
* Luna Cao  
* Mark Cook 
* Nicholas John Elder (nelder)
* Philip Kolman
* Abdulla Abdelkader Ouda
* Zhengyang Pan
* Pierce Saly
* Jeremy Wong


### Install Guide
1. Clone Project to Local Machine

```bash
git clone https://github.com/nelder/elixir
```

2. Install XAMPP to serve Apache webserver. The /webroot folder needs to be served as static content. 
3. Move project into apache webroot or at least ensure webroot folder is served on localhost using apache. 
4. The frontend is now being served.

### Install Flask (Python Backend)
1. Ensure Python3 is installed. 
2. Ensure mySQL is installed. 
3. Create database in mySQL with any name, like textbook_town. 
4. Add pip dependencies (while in Flask-backend folder) `sudo pip3 install -r requirements.txt`
5. Modify api.py in the backend folder with the correct mySQL information (constant DATABASE_LOGIN_STRING)
6. Run database install commands:

```python
nick@Nicks-MacBook-Pro-2:/Applications/XAMPP/xamppfiles/htdocs/elixir/Flask-backend$ python3
Python 3.4.3 (v3.4.3:9b73f1c3e601, Feb 23 2015, 02:52:03) 
[GCC 4.2.1 (Apple Inc. build 5666) (dot 3)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> from api import db
>>> db.create_all()
```

7. Quit to exit python3 interactive shell `quit()`
8. Run backend file:

```bash
nick@Nicks-MacBook-Pro-2:/Applications/XAMPP/xamppfiles/htdocs/elixir/Flask-backend$ python3 api.py 
 * Running on http://127.0.0.1:5000/
 * Restarting with reloader
```

9. Load frontent using localhost and apache webserver; rejoice as the website is now functional. We recommend trying: (click login, click register, register, login, add book to sell).

## Project Structure
* /docs [Our Website](https://textbook.town): for required team github page about us and our project.
* /webroot frontend javascript and designs.
* /Flash-backend is the backend logic and API to the frontend. It runs on python and mySQL.
* [Our Team Website](https://textbook.town): for required team github page about us and our project.