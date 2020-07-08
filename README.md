# JWT Authentication Server with Facebook and Google OAuth 
Token Authentication Server that utilizes JWT with Google/Facebook OAuth built on top of a Bootstrap frontend.

### Technology
* Python 
* Flask
* MySQL Connector
* HTML
* CSS
* JavaScript
* Bootstrap


### Setup
1. Set **MySQL database info** and **JWT token secrets** on `config.py`
2. Install required packages `pip install requirements.txt`
3. run Backend Server: ```python auth.py```
4. run Frontend: ``` python -m http.server```

### Libraries Used
* JWT
* Argon2 
* flask CORS
* MySQL Connector
* Google API Client
* Facebook JavaScript SDK


### Database Querying
Bulk query function - `query_all('SELECT * FROM users')` \
Single query function - `query_one('SELECT id FROM users where username = "test"')` \
Insert query function  
```
data = {
     'username': 'test',
     'password': 'test'
}

insert('INSERT INTO users (username, password) VALUES (%(username)s, %(password)s)', data)
```
