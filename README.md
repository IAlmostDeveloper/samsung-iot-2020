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

### Использование

