# Static_file_django

adding static file like javascript,css and another file we need to define static root in setting.py file
here are the step for including static file
1. open setting.py file and find static  url

```
STATIC_URL = '/static/'

```
2. create static folter insite app directory.
note: make sure the name of folder is static.
3. add static folder into root for that define code into setting.py givin below.

```
STATICFILES_DIRS = (     
os.path.join(BASE_DIR, 'static'), 
) 
STATIC_ROOT = os.path.join(BASE_DIR, 'staticfiles')

MEDIA_ROOT = os.path.join(BASE_DIR, 'media')
MEDIA_URL = '/media/'


```

