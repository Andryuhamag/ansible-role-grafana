`Ansible` роль для установки `Grafana`

------------
Пример использования:

```
---
- name: Install Grafana
  hosts: grafana-instance
  become: true
  roles:
    - role: ansible-role-grafana

```
При необходимости можно переопределить параметры подключения к `Prometheus`:
| Название параметра   | Описание                        | Значение по умолчанию |
|----------------------|---------------------------------|-----------------------|
| `prometheus_ds_host` | IP адрес сервера с `Prometheus` | `localhost`           |
| `prometheus_ds_port` | Порт сервера с `Prometheus`     | `9090`                |


