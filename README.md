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
