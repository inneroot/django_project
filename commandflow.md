#virtual env
source venv/bin/activate 
#itstall django
pip install django
# pips
pip install autopep8
---
pip install mccabe
pip install lazy-object-proxy
pip install isort
pip install astroid

#start django prj
django-admin startproject btre . 
#run server
python manage.py runserver 
# create Pages app
python manage.py startapp pages
# Add app to settings.py
'pages.apps.PagesConfig',
#URLS
create urls.py on pages
add include pages urls in btre urls.py
#Add TEMPLATES to settings.py
'DIRS': [os.path.join(BASE_DIR, 'templates')],
--> create folder templates
