# custom-user-model
Source code for django custom user model

**setting up environment**
```
<!-- for windows -->
python -m venv .
# activate
.\Scripts\activate (or) Scripts\activate
# deactivate
deactivate
```
``` 
<!-- for linux and mac -->
python3 -m venv .
# activte
source bin/activate
# deactivate 
deactivate
```

**Install Dependencies**
```
pip install django
```

**Setting up project**
```
# in root directory
django-admin startproject src .
python manage.py startapp account
```

**Create DataBase**
```
python manage.py makemigrations
python manage.py migrate
```

**Add installed app to settings.py**
```
INSTALLED_APPS = [
    ...
    'account.apps.AccountConfig',
    ...
]
```

**After creating custom user model**
```
# add it to settings.py 
AUTH_USER_MODEL = 'account.User'
```





MIT License

Copyright (c) 2021 Karthik Santhosh

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
