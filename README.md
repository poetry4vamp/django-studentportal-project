# django-studentportal-project

1. create a folder on your desktop, named it 'django'
2. go to the folder and type cmd on the folder path
3. type py -m venv venv
4. type venv\scripts\activate
5. type pip install django
6. update django version if needed
7. type django-admin startproject studentstudyportal
8. type cd studentstudyportal
9. type django-admin startapp dashboard
10. type code .
11. install python extension in vscode
12. type py manage.py createsuperuser (create your own admin credentials to access /admin)
13. type pip install django-crispy-forms
14. modify the INSTALLED_APPS of settings.py (see the 'settings.py' file in studentstudyportal folder)
15. add these at the bottom part of settings.py 

        STATIC_URL = '/static/'

        STATICFILES_DIRS=[BASE_DIR/"static"]

        CRISPY_TEMPLATE_PACK = "bootstrap4"
    
15. modify imports and urlpatterns of urls.py (see the 'urls.py' file in studentstudyportal folder)
16. type py manage.py makemigrations
17. type py manage.py migrate
18. if both makemigrations and migrate don't work, try to copy the files in migrations folder to your migrations folder
19. type py manage.py runserver 
    
    
    
