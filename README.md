Загрузка исходников
===================

Перед продолжением ознакомьтесь с [инструкциями по сборке AOSP](http://source.android.com/source/index.html).

Инициализация репозитория
-----------------------
    
Инициировать дерево Xiaomi Redmi 4X:

    $ repo init -u https://github.com/Areki-san/project_a.git

Синхронизировать репозиторий:

    $ repo sync --force-sync

***

Сборка
--------

После завершения синхронизации ознакомьтесь с [официальной инструкцией по сборке Android](http://s.android.com/source/building.html).

    . build/envsetup.sh
    lunch

Вы также можете создать сборку для конкретных устройств (например hammerhead):

    . build/envsetup.sh
    lunch aokp_hammerhead-userdebug
    mka rainbowfarts

Не забывайте делать `make clobber && make clean` время от времени!