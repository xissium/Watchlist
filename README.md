# Watchlist

An easy application use Python, Flask and MySQL.

## Installation

1. clone:

```
git clone https://github.com/xissium/watchlist.git
cd watchlist
```

2. create & active virtual environment then install dependencies:

```
python -m venv env
# or use conda
# conda create -n watchlist python=3.9
pip install -r requirements.txt
```

3. change MySQL configuration info in `src/__init__.py`:

```
app.config['SQLALCHEMY_DATABASE_URI'] = 'mysql+pymysql://{user}:{password}@{host}[:{port}]/watchlist'
```

4. create a database named `watchlist`:

```
CREATE DATABASE `watchlist` DEFAULT CHARACTER SET utf8mb4;
```

5. generate fake data then run:

```
flask forge
flask run
```

