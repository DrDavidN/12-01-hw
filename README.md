# «Kubernetes. Причины появления. Команда kubectl» - Дрибноход Давид

### Задание 1. Установка MicroK8S

1. Установить MicroK8S на локальную машину или на удалённую виртуальную машину.
2. Установить dashboard.
3. Сгенерировать сертификат для подключения к внешнему ip-адресу.

#### Ответ:
1. Устанавливаю MicroK8S
``` sudo apt install snapd ```
``` sudo snap install microk8s --classic ```
![image](https://github.com/DrDavidN/12-01-hw/assets/128225763/beb4ab29-03de-48d1-ac22-39e631f54b82)
![image](https://github.com/DrDavidN/12-01-hw/assets/128225763/2728c30f-97bb-4478-ac50-6c559a0f509c)

``` microk8s status --wait-ready ```
![image](https://github.com/DrDavidN/12-01-hw/assets/128225763/0f7639a6-66d6-44e4-8aba-eb133083f7b3)

3. Устанавливаю dashboard.
![image](https://github.com/DrDavidN/12-01-hw/assets/128225763/2477b633-643c-4980-b854-6d5ef97830bc)

4. Обновляю сертификат предварителььно добавив внешний адрес в файл конфигурации /var/snap/microk8s/current/certs/csr.conf.template
![image](https://github.com/DrDavidN/12-01-hw/assets/128225763/90f57e84-bd7f-4fc1-927f-867f22f7aa7f)
![image](https://github.com/DrDavidN/12-01-hw/assets/128225763/5adb358c-76f1-4257-97a4-e170d73edbc6)

------

### Задание 2. Установка и настройка локального kubectl
1. Установить на локальную машину kubectl.
2. Настроить локально подключение к кластеру.
3. Подключиться к дашборду с помощью port-forward.

#### Ответ:
1. Устанавливаю kubectl
![image](https://github.com/DrDavidN/12-01-hw/assets/128225763/bfd4fd36-b726-4315-aebb-8a39052a7561)

2.Запустил port-forward и получил токен для подключения
![image](https://github.com/DrDavidN/12-01-hw/assets/128225763/fc7cc525-c18b-4bc0-aaac-5c6d08a7db48)
![image](https://github.com/DrDavidN/12-01-hw/assets/128225763/6217f71a-b08c-486e-8b4e-96b6b98c6d15)

3. Подключился к дашборду с помощью port-forward.
![image](https://github.com/DrDavidN/12-01-hw/assets/128225763/ae486b78-6958-40f7-8f27-d0d9d23203ab)

------
