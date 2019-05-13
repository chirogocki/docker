### Inventory variables

| Variables | Values |
|----------|:---------:|
| keepalived_role | MASTER or BACKUP |
| keepalived_auth_pass | password 8 char string |
| keepalived_router_id | numerical value |
| keepalived_shared_iface | host ethernet name.<br/>Centos default ex : ens160 |
| keepalived_shared_ip | VIP |
| keepalived_check_process | Service name to check<br/>ex : keepalived |
| keepalived_priority | Priority for master node<br/>ex : 100 |
| keepalived_backup_priority | Priority for backup node<br/>ex : 50 |