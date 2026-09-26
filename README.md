# vector-role

Устанавливает Vector из tar.gz и настраивает systemd-сервис.

## Переменные (defaults)

| Переменная | Значение по умолчанию |
|---|---|
| `vector_version` | `0.42.0` |
| `vector_arch` | `x86_64-unknown-linux-gnu` |
| `vector_install_dir` | `/opt/vector` |
| `vector_config_dir` | `/etc/vector` |
| `vector_data_dir` | `/var/lib/vector` |
| `vector_user` | `vector` |
| `vector_group` | `vector` |

## Использование

```yaml
- hosts: vector
  become: true
  roles:
    - vector-role
