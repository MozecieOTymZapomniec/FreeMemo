cy - my side business webpage source code
-09.06.2023 - fixer.cy page is down due to hosting change -

 Q: Why do I share it to you?

 A: Actually, I am sharing it to my potential PRIMARY business partners (who are looking for skilled DevOPS engineers) to show them my Python/SQLAlchemy/Postgres skills level :) But if you find my code useful, feel free to explore and use it!


# Prerequisites:
0. Linux/MacOS/WSL 2
1. Python3
2. PostgreSQL database up and running


# Installation:
Create virtual environment in your python setup:

0. pwd -> (should return): ||SOMETHING||/Fixer  
1. cd ./run
2. python3 -m venv venv
3. virtualenv -p python3 venv
4. source venv/bin/activate
5. (venv) $ pip install flask flask-wtf flask-sqlalchemy flask-migrate psycopg2-binary flask-login email-validator flask-socketio python-dotenv


Set database URL (you need to install and create PostgresSQL database named 'fixer_db', expose its port and create user 'fixer' who has all privileges granted to 'fixer_db' database ), after that create new environment variable called DATABASE_URL as below, but put your database credential inside <...> fields

(venv) $ DATABASE_URL="postgresql://fixer:<FREEMEMO_USER_PASSWORD>@<DATABASE_IP>:<DATABASE_PORT>/fixer_db"

# Run
(venv) $ flask run --host=0.0.0.0 -p 1990

use the port 1990 or the other that you choose :)
