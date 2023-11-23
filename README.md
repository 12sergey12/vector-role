Vector-role
=========

Предназначена для установки на операционные системы под управлением SystemD сервиса Vector и базовое конфигурирование отслеживания изменения LOG файлов с отправкой изменений в Clickhouse

Requirements
------------

1. Ubuntu ОС
2. Предустановленная БД Clickhouse.

Role Variables
--------------

vector_version - Версия используемого ПО Vector. По умолчанию 0.34.1-1

Dependencies
------------

Для установки Clickhouse требуется роль ansible-clickhouse: https://github.com/AlexeySetevoi/ansible-clickhouse

Example Playbook
----------------

Пример добавление роли в playbook:

```
- name: Install Vector
  tags: [vector]
  hosts: vector
  roles:
    - vector-role
```

License
-------

BSD

Author Information
------------------

Baranov Sergey
