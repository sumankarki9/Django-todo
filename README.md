# django-todo
A simple todo app built with django

### Setup
## Usage Instructions
To get this repository, Clone this repository by run the following command inside your git enabled terminal
```bash
$ https://github.com/sumankarki9/django-todo-app.git
```

Once you cloned repo, go to the cloned repo directory and run the following command

```bash

$ cd django-todo # Moving into the project folder

$ virtualenv -p python3 env # Creating virtual environment

$ source env/bin/activate # To activate virtual-environment ; Type deactivate to deactivate the virtual environment

$ Install Django

# Possible Errors May Come:
# Time Zone Error Then 
$ cd todoApp 

$ sudo vim settings.py 

# Change Timezone to: 'Asia/Kathmandu'

# DisallowedHost at Invalid HTTP_HOST header: '127.0.0.1:8000'. You may need to add '127.0.0.1' to ALLOWED_HOSTS.

$ sudo vim settings.py

# Change ALLOWED_HOSTS = ['127.0.0.1']

$ python manage.py makemigrations
```
This will create all the migrations file (database migrations) required to run this App.

Now, to apply this migrations run the following command
```bash
# test
$ python manage.py migrate
```
One last step and then our todo App will be live. We need to create an admin user to run this App. On the terminal, type the following command and provide username, password and email for the admin user
```bash

$ python manage.py createsuperuser
```
That was pretty simple, right? Now let's make the App live. We just need to start the server now and then we can start using our simple todo App. Start the server by following command

```bash

$ python manage.py runserver
```

Once the server is hosted, head over to http://127.0.0.1:8000/todos for the App.

Cheers and Happy Coding :)
# django-todo-updated
