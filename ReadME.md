## Django Rest Framework (DRF)
Get started with DRF
- ``pip install djangorestframework``
- In ProjectName -> `settings.py`
```
INSTALLED_APPS = [
    ...
    'rest_framework',
]
```

- To start a app run the command
`python manage.py startapp <appname>`

- Now add this app also in the `settings.py` file
```
INSTALLED_APPS = [
    ...
    'rest_framework',
    '<appname>',
]
```
---
You are done with the basic setup
---
Here are few libraries you need to import
Copy paste as it is in the `<appname> -> views.py`
```
from rest_framework.renderers import JSONRenderer
from rest_framework.parsers import JSONParser
from django.http import HttpResponse
from django.http import JsonResponse
from django.views.decorators.csrf import *
``` 