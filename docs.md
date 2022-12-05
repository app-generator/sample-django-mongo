# [Django Material Kit MongoDB]()
This is django+Material Kit+ MongoDB starter template

## Requirements
Project depends on these exact versions of dependencies to work.
- Python 3.9
- django==3.2.16
- djongo==1.3.6
- dnspython==2.2.1
- pymongo==3.12.1
- Git
  
You need MongoDB setup locally or online as per your preference

## MongoDB Setup <br>
### **Local Server Setup**<br>
**Step 1👉Local MongoDB database Setup**



MongoDB Community Server Download Page [Here](https://www.mongodb.com/try/download/community).

Download  and Install the server

**Windows users**

Go to MongoDb download page and download `.msi` installer package for windows.
Run the installer and install complete package a


On successful MongoDB Community server download, add `MONGO_DATABASE` and `MONGO_SERVER_CLUSTER_URL` in the `.env` file.

**TIP 👉**  You can install MongoDB Compass to aid in querying the database using a GUI.

On successful installation create a database.

**Step 2 👉** Add environmental variables to your `.env` file

```
MONGO_DATABASE=<mongo_database_name>
MONGO_SERVER_CLUSTER_URL=<Mongo_atlas_database_url>
```
### **Atlas MongoDB Setup**

**Step 1 👉Atlas MongoDB database Setup**
Login to your atlas account and create your database cluster according to your project needs but you can start with a free shared database  [Atlas MongoDB Account Here](https://cloud.mongodb.com)

<img width="100%"  src="./images/Screenshot%202022-11-30%20232705.png">

On successful creation of Atlas Cluster it will be visible as Cluster

<img width="100%"   src="./images/Screenshot 2022-11-30 232846.png">


Copy the connection string for connecting using python as the language

<img width="100%"   src="./images/Screenshot%202022-11-30%20233728.png">


**Step 2 👉** Add environmental variables to your `.env` file

```
DEBUG=True
MONGO_DATABASE=<mongo_database_name>
MONGO_SERVER_CLUSTER_URL=<MongoDB Cluster URL>
```

## Getting Started
 **Step 1** - Download the code from the GH repository (using `git`) 

 It comes preinstalled in Unix and Mac.<br>
 If you dont have `git` installed on your system download and install it [Git Download Page](https://git-scm.com/downloads)

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




