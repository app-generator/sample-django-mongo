# [Django Material Kit MongoDB]()
This is django+Material Kit+ MongoDB starter template

## Requirements
Project depends on these exact versions of dependencies to work.
- django==3.2.16
- djongo==1.3.6
- dnspython==2.2.1
- pymongo==3.12.1
  
You need MongoDB setup also



## MongoDB Setup <br>
### **Local Server Setup**<br>
**Step 1👉Local MongoDB database Setup**
follow Mongodb Installation requirements to install it in your system. 

**TIP 👉**  You can install MongoDB Compass to aid in querying the database using a GUI.

On successful installation create a database.


**Step 2 👉** Add environmental variables to your `.env` file

```
MONGO_DATABASE=<mongo_database_name>
```
### **Atlas MongoDB Setup**


**Step 1 👉Atlas MongoDB database Setup**
Login to your atlas account and create your database cluster

**Step 2 👉** Add environmental variables to your `.env` file

```
MONGO_DATABASE=<mongo_database_name>
MONGO_SERVER_CLUSTER_URL=<MongoDB Cluster URL>
```

## Getting Started
 **Step 1** - Download the code from the GH repository (using `GIT`) 

```bash
$ git clone https://github.com/app-generator/sample-django-mongo.git
```


 **Step 2 -** - create virtual environment and install project dependencies

** 👉Linux/MacOS Users Setup**

Open Terminal and navigate to the repo
```bash
$ cd sample-django-mongo
$ pip install virtualenv
$ python-virtualenv env
(env) $ pip install -r requiremants.txt

```

**👉 Windows Users Setup**

Open Windows Powershell or CMD and navigate to the repo
```powershell
C:\> cd sample-django-mongo
C:\> pip install virtualenv
C:\> python-virtualenv env
C:\> env\Scripts\activate
(env) C:\> pip install -r requiremenrs.txt

```

### Runing the Project
To run the project all you need to do is run the command

 ```bash
 $ python manage.py makemigrations
 $ python manage.py migrate
 $ python manage.py runserver
 ````

Now open the browser and navigate to [localhost:8000](http://localhost:8000) and the application should be up and running.


## Addons
For manual Django and MongoDb intergration you can read the docs [Here](https://www.mongodb.com/compatibility/mongodb-and-django)


