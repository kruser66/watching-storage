# Публикуем комиксы во ВКонтакте
Модуль предназначен для постинга случайного комикса с https://xkcd.com/ на стену в сообщество ВКонтакте.


# Как установить

Python3 должен быть уже установлен. Затем используйте pip (или pip3, если есть конфликт с Python2) для установки зависимостей:

```Python
pip install -r requirements.txt
```

### Переменные окружения
Для корректной работы модуля необходимы следующие переменные окружения:

```Python
VK_ACCESS_TOKEN='YourVKAppAccessToken'
```
1. Создать приложение в VK.
2. По номеру приложения `client_id` используя [Implicit Flow](https://dev.vk.com/api/access-token/implicit-flow-user) получить `access_token`
3. Необходимы права `photos`, `groups`, `wall` и `offline`

```Python
VK_PUBLIC_ID='YourVKPublicId'
```
ID группы, в которую буду поститься комиксы.

### Пример запуска

```
python xckd-vk.py
``` 

# Цель проекта

Код написан в образовательных целях на онлайн-курс для веб-разработчиков [Devman](https://dvmn.org/).