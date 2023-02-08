### Гайд по настройке Gosha.ova file

#### 1. Скачиваем Gosha.ova file 
```
Актуальные версии Gosha.ova (на 06.02.2023): 
        1) Для домашнего использования - v.1.7
        2) Для учебных учреждений - v1.8
```
"Что понадобится?" :
```
1. "Электронный носитель" :
        Тут есть несколько вариантов:
            1) Флешка (на 64 Гигабайт)
            2) Внешний жёсткий диск (С остатком 40+ гигабайт свободного места)
            3) Жёсткий диск (HDD) или же твердотельный накопитель (SSD) (С остатком 40+ гигабайт свободного места)

    2. "Ваше присутствие в" :
            Тут есть несколько вариантов:
                1) 302/4 (Евсеева В.В.)
                2) 306/4 (Сулейманов С.В.)

        3. "Ваша просьба к преподавателям из пункта 2" 
```

#### 2. Установка Gosha.ova file (Deploy)
"Что понадобится?" :
```
1. "Девайс"
        Тут есть несколько вариантов: 
            1) PC 
            2) Ноутбук
            3) Остальные устройства
    
    2. "Минимальные характеристики девайса" :
        1) ЦП - 4 ядра
        2) ОЗУ - 8 Гигабайт
        3) HDD/SSD - 235 Гигабайт
```



"Как это сделать?" :
```
(Ранее на вашем устройстве должна быть установлена и активирована программа Vmware Workstation)
1) Кликаете два раза ЛКМ по файлу Gosha.ova :
```
![image](/screenshots/ssl1.png)
```
2) Выдаёте "любое" название виртуальной машине (Н-Р: DEMO), и указываем путь где будет находиться виртуальная машина - Import :
```
![image](/screenshots/ssl2.png)
```
3) Ждём пока заимпортируется виртуальная машина: 
```
![image](/screenshots/ssl3.png)
```
4) ПКМ по виртуальной машине - Settings... : 
```
![image](/screenshots/ssl4.png)
```
5) ПКМ по Network Adapter - Bridged... - Replicate... - OK :
```
![image](/screenshots/ssl5.png)
```
6) Options:
```
![image](/screenshots/options1.png)
```
7) Выбираем операционную систему Vmware ESX - VMware ESXI 7 - OK :
```
![image](/screenshots/options2.png)
```
8) Включаем виртуальную машину
    9) Нажимаем F2 :
```
![image](/screenshots/ssl6.png)
```
10) Вводим пароль (P@ssw0rd)
    11) Нажимаем Enter : 
```
![image](/screenshots/ssl7.png)
```
12) Спускаемся до пункта Configure Management Network - Enter :
```
![image](/screenshots/ssl8.png)
```
13)  Спускаемся до пункта IPv4 Configuration - Enter :
```
![image](/screenshots/ssl9.png)
```
14) Выбираем Set static IPv4 address  and network configuration :
    15) Выдаём "любой; свободный ip адрес; из той же подсети - в которой находится Default Gateway" (Н-Р: 192.168.202.100) : 
        16) Выдаём маску подсети (Н-Р: 255.255.255.0) :
            17) Прописываем Defauly Gateway (ip адрес роутера - через который вы сидите) :
                18) Нажимам Enter :
```
![imnage](/screenshots/ssl10.png)
```
19) Esc : 
```
![image](/screenshots/ssl11.png)
```
20) Y : 
```
![image](/screenshots/ssl12.png)
```
21) Спускаемся до пункта Restart Management Network - Enter :
```
![image](/screenshots/ssl13.png)
```
22) F11 :
```
![image](/screenshots/ssl15.png)
```
23) Enter :
```
![image](/screenshots/ssl16.png)

#### 3. Проверка работы стенда
```
1) Открываем барузер и вписываем ранее выданный адрес виртальной машины - Enter:
```
![image](/screenshots/status1.png)
```
2) Нажимаем Advanced :
```
![image](/screenshots/status2.png)
```
3) Нажимаем Proceed to 192.168.202.122 (unsafe) : 
```
![image](/screenshots/status3.png)
```
4) Наблюдаем работающую web страничку стенда на вашем устройстве : 
```
![image](/screenshots/status4.png)

#### 4. Подключение к стенду
```
1) На страничке Home нажимаем Connect to a Remote Server :
```
![image](/screenshots/con1.png)
```
2) Вводим данные подключения - Connect :
```
![image](/screenshots/con2.png)
```
3) Connect Anyway :
```
![image](/screenshots/con3.png)
```
4) Наблюдаем работающий стенд на вашем устройстве : 
```
![image](/screenshots/con4.png)

#### 5. Создание snapshot`ов
```
1) Нажимаем на Take a snapshot of this virtual machine :
```
![image](/screenshots/snapshot.png)
```
2) Выдаем имя (Н-Р: Default) - Take Snapshot :
```
![image](/screenshots/snapshot1.png)
```
3) Ждём пока создастся snapshot : 
```
![image](/screenshots/snapshot2.png)

#### 6. Работа с snapshots (revert)
1. Если вы создали только один snapshot
```
1) Нажимаем на Revert this virtual machine to snapshot: Default :
```
![image](/screenshots/revert1.png)

2. Если вы создали несколько snapshot`ов 
```
1) Нажимаем на Manage snapshots for this virtual machine :
```
![image](/screenshots/revert2.png)
```
2) Нажимаете на нужный snapshot - Go To :
```
![image](/screenshots/revert3.png)
```
3) Yes :
```
![image](/screenshots/revert4.png)
```
4) Ждём пока стенд откатится :
```
![image](/screenshots/revert5.png)

