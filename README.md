# samsung-iot-2020
Исходники, презентация и видос к финалу проектов по иоту

Скоро тут будет описание проекта, если я не забью

Части проекта:
- Сервер: https://github.com/IAlmostDeveloper/remote-control-server/blob/master/README.md
- Клиент(Android-приложение): https://github.com/IAlmostDeveloper/remote-control-android/blob/master/README.md
- Прошивка контроллера: https://github.com/IAlmostDeveloper/remote-control-esp/blob/master/README.md

# Как использовать

## Сервер
Сервер необходимо только запустить по инструкции по ссылке: https://github.com/IAlmostDeveloper/remote-control-server/blob/master/README.md

## Прошивка
Контроллер прошивается по инструкции по ссылке: https://github.com/IAlmostDeveloper/remote-control-esp/blob/master/README.md

### Как настроить: 
При первом запуске(либо после хард ресета) контроллер включает режим точки доступа (стандартный пароль 12345678). 
- Необходимо подключиться к точке доступа и перейти по адресу 192.168.4.1
- Затем выполнить настройку подключения к интернету и MQTT-брокеру. 
- После успешного подключения к MQTT загорится светодиод индикации. Теперь устройство готово принимать и передавать сигналы.
### Soft/Hard Reset
В устройстве есть функция мягкого и жесткого перезапуска. 
- Soft reset - простой перезапуск устройства. 
- Hard reset - перезапуск устройства и сброс его настроек. После Hard reset контроллер необходимо снова подключить к интернету/mqtt через страницу его настроек по адресу 192.168.4.1

## Клиент(Android-приложение)
- Приложение можно собрать в Android Studio по инструкции https://github.com/IAlmostDeveloper/remote-control-android/blob/master/README.md
- Готовый APK файл приложения лежит в репозитории: https://github.com/IAlmostDeveloper/samsung-iot-2020/blob/main/sources/Android%20Client/remote-control.apk

## Использование

### Страница логина на сервере (сервер можно поднять самому и указать его адрес)
### Примечание: пока что есть баг, изза которого нужно перезапустить приложение после смены адреса сервера.

![](https://i.ibb.co/ykCbKG6/photo-2020-11-07-14-30-40.jpg)

После логина откроется страница со списком контроллеров.
- Можно добавить новый контроллер: 

![](https://i.ibb.co/gWJLYzB/photo-2020-11-07-14-30-43.jpg)
![](https://i.ibb.co/y0STrqw/photo-2020-11-07-14-30-44.jpg)
![](https://i.ibb.co/SyJRNrX/photo-2020-11-07-14-30-44-2.jpg)

### Добавление кнопки в контроллер:
- Можно ввести код кнопки вручную
- Можно нажать кнопку "Get code from receiver", затем направить старый пульт от тв/аудиосистемы/прочего на приемник контроллера.
- Код появится в приложении сам

![](https://i.ibb.co/0CjRq4G/photo-2020-11-07-14-30-45.jpg)
![](https://i.ibb.co/VD3V8zf/photo-2020-11-07-14-30-45-2.jpg)
![](https://i.ibb.co/mzw4W0T/photo-2020-11-07-14-30-46.jpg)
![](https://i.ibb.co/0h6yqQ7/photo-2020-11-07-14-30-47.jpg)

- Нажимаем кнопку Apply, в контроллере появится новая созданная кнопка с нужным нам кодом.

![](https://i.ibb.co/Q8KKB8d/photo-2020-11-07-14-30-48.jpg)

### Возможность создавать скрипты

![](https://i.ibb.co/yV0wVXJ/photo-2020-11-07-14-30-48-2.jpg)
![](https://i.ibb.co/2ybtyk4/photo-2020-11-07-14-30-49.jpg)

