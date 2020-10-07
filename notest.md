https://www.djangoproject.com/

```
pip install Django

python -m django --version

```

1. Tworzenie nowego projektu > przy pomocy pliku django-admin.py

przechodzimy do katalogu w ktorym chcemy utworzyc projekt 
```
python django-admin startproject nazwa_projektu
``` 

2. Uruchomienie servera w lokalizacji gdzie jest plik manage.py aby sprawdzic czy projekt dobrze się zainstalował
``` 
python manage.py runserver
```

3. utworz nowa aplikacje  
```
python manage.py startapp nazwa_aplikacji
```

4. Przygotowanie bazy danych

otwieramy plik settings.py i ustawiamy LANGUAGE_CODE = 'pl'

trzeba ustawić dane dotyczace bazy danych :

'ENGINE': 'django.db.backends.sqlite3',
        'NAME': BASE_DIR / 'db.sqlite3',
        
baze sqlite mozna aprzegladac na firefox  >> https://addons.mozilla.org/pl/firefox/addon/sqlite-manager-webext/

tworzenie tabel:
```
python manage.py migrate
```

aktualizacji np modeli:
```
python manage.py makemigrations
```


