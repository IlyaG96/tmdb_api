# Программа для нахождения похожего фильма

Знакомо то чувство, когда только что закончил смотреть очередной великолепный фильм, и хочешь если не продолжения, то чего-то подобного? 

Решение проблемы существует: поиск "похожих" фильмов в базе данных themoviedb.org


#### Что понадобится?
+ Установленная версия python
+ пакеты ordereddict, requests
+ учетная запись IMDb
+ IMDb token

#### Как с этим работать? Часть 1
Клонируйте этот репозиторий себе на компьютер или скачайте его, создайте новое виртуальное окружение в папке с репозиторием командой
**python -m venv env**.  
Активируйте виртуальное окружение командой **source env/bin/activate**  
Установите пакеты ordereddict и requests **pip install <название пакета>**  

#### Как с этим работать? Часть 2
Теперь самое время получить токен TMDb
Перейдите вот сюда: https://www.themoviedb.org/ и зарегистрируйтесь. Затем нажмите на значок своего профиля в правом верхнем углу --> "параметры"
Слева найдите пункт "API".  
Заполняйте все необходимые поля, следуя инструкциям, получайте Ключ API подобного вида: "998874lklknde13e380084asdkmff08e".

#### Как с этим работать? Часть 3
Отлично, ключ API получен. 
Запустите файл make_own_db.py командой **python make_own_db.py**.   

- *Enter your api key v3* - введите свой Ключ API (v3 auth) c сайта.
- В течение 10-15 минут будет создана база данных с 1000 фильмов

Запустите файл find_similar.py командой **python find_similar.py**

- Введите название фильма на английском и, если этот фильм есть в базе данных, вы увидите список схожих с ним фильмов.
- Наслаждайтесь просмотром

#### Возможные проблемы с ssl на MacOs:

- https://stackoverflow.com/questions/50236117/scraping-ssl-certificate-verify-failed-error-for-http-en-wikipedia-org










