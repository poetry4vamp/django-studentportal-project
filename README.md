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
12. type pip install django-crispy-forms
13. type py manage.py makemigrations
14. type py manage.py migrate
15. modify settings.py (see the 'settings.py' file in studentstudyportal folder)

INSTALLED_APPS = [
...
'dashboard',
'crispy_forms'
'crispy_bootstrap4'
]

16. add these at the bottom part of settings.py 

STATIC_URL = '/static/'
STATICFILES_DIRS=[BASE_DIR/"static"]
    
CRISPY_TEMPLATE_PACK = "bootstrap4"
    
17. modify urls.py (see the 'urls.py' file in studentstudyportal folder)

from django.urls.conf import include
    
urlpatterns = [
...
path('',include('dashboard.urls'))
]

18. type py manage.py runserver
    
    
    
