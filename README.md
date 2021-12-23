# POS = Point of sales
> The web application is simple Point of sales and inventory management system web-app.
 #### Features:
 Configuration:
 -  Inventory Categories
 -  Inventory Sub Category
 -  Inventory Tag
 
 Inventory Information:
 - Inventory name 
 - Inventory short description  
 - Inventory full description  
 - Inventory category selection  
 - Inventory picture 
 - Inventory current stock
 - Inventory purchase price
 - Inventory sales price
 - Inventory promotional price
 
 POS:
 - Product Sales
 - List of sale record
 - Invoice 

### Test User Creds:

```
Username = test
Password = 1q2w3e4r5t6y.
```

## Setup & dependencies

- Python 3.8.5 and above
- Django 3.1.2 and above
- Postgres 12.5 and above

The following steps will walk you thru installation on a Mac. Linux should be similar.
It's also possible to develop on a Windows machine, but I have not documented the steps.
If you've developed django apps on Windows, you should have little problem getting
up and running.


### Create Database

Create the database by running the following commands in a psql shell. If you're using
Postgres.app, click the Postgres.app icon in your toolbar and select "Open psql".

or 

Open Terminal. then type psql

```
create database "inventory";

```


### Setup Django Server (Mac)

We're using python3 instead of python2.x. If you don't have python3 installed,
install [Homebrew](http://brew.sh), then…

```
brew install python3.8

or

sudo apt install python3
```

Assuming you've cloned the repository, open Terminal and `cd ~/your/path/to/inventory`.

Create a python virtual environment:

```bash
python -m  venv envpos --python=python3.8
```

Activate it:

```bash
source envpos/bin/activate
```

Install the python dependencies which includes django and other libraries.

```
pip3 install -r requirements.txt
```


## Run server locally

```
python3 manage.py migrate
python3 manage.py runserver
```

###### If PSQL error raise please follow the command:
```pip install psycopg2-binary```

