# docker based grafana+influx for icinga2 integration deployment using ansible
See playbooks, set your variables and enjoy

```sh
$COPS_ROOT/bin/ansible-playbook -vvv -i $inv deploy.yml \
    -e "{grafana_servers: dockergrafana_servers, cops_vars_debug: true}" \
    --skip-tags docker_setup,grafana_service_stop,configuree,grafana_service_starte,post
```
