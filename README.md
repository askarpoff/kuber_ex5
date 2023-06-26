# Домашнее задание к занятию «Сетевое взаимодействие в K8S. Часть 2»

### Задание 1. Создать Deployment приложений backend и frontend

1. Создать Deployment приложения _frontend_ из образа nginx с количеством реплик 3 шт.
   
2. Создать Deployment приложения _backend_ из образа multitool.
  
3. Добавить Service, которые обеспечат доступ к обоим приложениям внутри кластера.
 
![image](https://github.com/askarpoff/kuber_ex5/assets/108946489/062252e2-787f-4486-841d-2c83bb523cf8)
 
4. Продемонстрировать, что приложения видят друг друга с помощью Service.

![image](https://github.com/askarpoff/kuber_ex5/assets/108946489/fb9a664a-3244-4b5d-b2df-f867f2e50618)
   
5. Предоставить манифесты Deployment и Service в решении, а также скриншоты или вывод команды п.4.

[frontend.yaml](https://github.com/askarpoff/kuber_ex5/blob/main/task1/frontend.yaml)

[backend.yaml](https://github.com/askarpoff/kuber_ex5/blob/main/task1/backend.yaml)

[services.yaml](https://github.com/askarpoff/kuber_ex5/blob/main/task1/services.yaml)

------

### Задание 2. Создать Ingress и обеспечить доступ к приложениям снаружи кластера

1. Включить Ingress-controller в MicroK8S.
```bash
microk8s enable ingress
```
3. Создать Ingress, обеспечивающий доступ снаружи по IP-адресу кластера MicroK8S так, чтобы при запросе только по адресу открывался _frontend_ а при добавлении /api - _backend_.
4. Продемонстрировать доступ с помощью браузера или `curl` с локального компьютера.
5. Предоставить манифесты и скриншоты или вывод команды п.2.

------

## Ответ:

### Задание 1. Создать Deployment приложений backend и frontend

1. Создать Deployment приложения _frontend_ из образа nginx с количеством реплик 3 шт.
2. Создать Deployment приложения _backend_ из образа multitool. 
3. Добавить Service, которые обеспечат доступ к обоим приложениям внутри кластера. 
4. Продемонстрировать, что приложения видят друг друга с помощью Service.
5. Предоставить манифесты Deployment и Service в решении, а также скриншоты или вывод команды п.4.

------

### Задание 2. Создать Ingress и обеспечить доступ к приложениям снаружи кластера

1. Включить Ingress-controller в MicroK8S.
2. Создать Ingress, обеспечивающий доступ снаружи по IP-адресу кластера MicroK8S так, чтобы при запросе только по адресу открывался _frontend_ а при добавлении /api - _backend_.
3. Продемонстрировать доступ с помощью браузера или `curl` с локального компьютера.
4. Предоставить манифесты и скриншоты или вывод команды п.2.

