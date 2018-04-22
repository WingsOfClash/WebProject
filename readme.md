**How to run the app (localhost)**
First of all make sure that you have all the packages of the requeriments.txt file.
Then check that your python version is python-2.7.14

Finally:

```$ python manage.py runserver```

**How to create an admin user**
For create an admin user use the next command:

```$ python manage.py createsuperuser```

There is an admin created for testing the web:

- User: Test
- Password: Testing123

**How to deploy the apliccation on Heroku** 

- Init a git repository:
 ```$ git init```

- Add all the files and commit them:
```
$ git add .

$ git commit -m "Message"
```

- Login with heroku:

```$ heroku login```

- Create an aplication:

```$ heroku create```

- Deploy the code:

```$ git push heroku master```

- Scale the web:

```$ heroku ps:scale web=1```

- On settings.py you have to add your host on ALLOWED_HOSTS, example:
Settings.py:

```ALLOWED_HOSTS = ['tomas123.herokuapp.com']```

Web example: https://tomas123.herokuapp.com/dogapp/
