# Домашнее задание к занятию 6. «Оркестрация кластером Docker контейнеров на примере Docker Swarm»



[Ссылки для установки открытого ПО](https://github.com/netology-code/devops-materials/blob/master/README.md).

---

## Задача 1

Создайте ваш первый Docker Swarm-кластер в Яндекс Облаке.
Документация swarm: https://docs.docker.com/engine/reference/commandline/swarm_init/
1. Создайте 3 облачные виртуальные машины в одной сети.
2. Установите docker на каждую ВМ.
3. Создайте swarm-кластер из 1 мастера и 2-х рабочих нод.

4. Проверьте список нод командой:
```
docker node ls
```

## Решение 1

MASTER
![yc compute instance master node](https://github.com/user-attachments/assets/72c65af9-3fdb-4a35-b4c1-e2b18fc9752f)
---

WORKER1
![yc worker1](https://github.com/user-attachments/assets/3265a901-8813-48a4-aab5-71f58ba2f04f)
---

WORKER2
![yc worker2](https://github.com/user-attachments/assets/b1daf813-9974-4ff6-9880-c0918c53112a)
---


## Задача 2 (*) (необязательное задание *).
1.  Задеплойте ваш python-fork из предыдущего ДЗ(05-virt-04-docker-in-practice) в получившийся кластер.
2. Удалите стенд.


## Задача 3 (*)

Если вы уже знакомы с terraform и ansible  - повторите практику по примеру лекции "Развертывание стека микросервисов в Docker Swarm кластере". Попробуйте улучшить пайплайн, запустив ansible через terraform синамическим инвентарем.

Проверьте доступность grafana.

Иначе вернитесь к выполнению задания после прохождения модулей "terraform" и "ansible".
