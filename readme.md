This is a Django template with a custom User model that **uses email as username** and does not require the username field to be filled in while signing up.

The code has been written following this tutorial:
https://www.fomfus.com/articles/how-to-use-email-as-username-for-django-authentication-removing-the-username/

The custom User is created using the built-in AbstractUser model in Django and the model manager is built using the BaseUserManager.

Since it is difficult to change the User model once created, makemigrations has not been run in this repl.
If you do not wish to make any changes to the code for the User & UserManager, proceed with the following steps:

1. Press "Run" (to run Django. Don't worry if there are some errors in the console at this stage)
2. Press "Stop"
3. `$ python manage.py makemigrations emailasuser`
4. `$ python manage.py migrate`
5. Create a superuser account with `$ python manage.py createsuperuser`
6. Press "Run".
7. Proceed to "repl-url/admin" and login with your superuser credentials.