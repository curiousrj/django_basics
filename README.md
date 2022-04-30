# djange_basics

create project - django-admin startproject projectname<br/>
create app - django-admin startapp appname<br/>
start server - python manage.py runserver<br/>
url mapping - urlpatterns = [ path('',include('appname.urls')), path('',views.functionname,name='functionname') ]<br/>
set templates address - 'DIRS': [os.path.join(BASE_DIR,'templates')]<br/>
show page - return render(request,'pagename.html')<br/>
code reuse -<br/>
{% block content %}<br/>
{% endblock %}<br/>
{% extends 'pagename.html' %}<br/><br/>
{% block content %}<br/>
{% endblock %}<br/>
get value from html - request.POST['name']<br/>
CSRF Protection - {% csrf_token %}<br/>
static files -<br/>
STATICFILES_DIRS = [<br/>
os.path.join(BASE_DIR,'foldername where files are available') ]<br/>
STATIC_ROOT = os.path.join(BASE_DIR,'newfolder to create')<br/>
static files command - python manage.py collectstatic<br/>
include static to index page -<br/>
{% load static %}<br/>
href="{% static 'path' %}"<br/>
pass value to page - return render(request, 'index.html', {'name as pass': name of variable})<br/>
import something from same folder - from .modelname import class or model<br/>
for loop in html page -<br/>
{% for variable in list %}<br/>
...content...<br/>
{% endfor %}<br/>
if statement in html page -<br/>
{% if condition %}<br/>
...content...<br/>
{% endif %}<br/>
