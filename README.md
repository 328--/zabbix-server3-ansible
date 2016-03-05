Zabbix 3.0.1 用 ansible

# how to use

- playbook.ymlのvarsにmysqlのroot,zabbixユーザのパスワードを記述してください
- hostsにzabbix-serverを構築するServerのIPアドレスを記述してください


# 実行

```
ansible-playbook -i hosts playbook.yml --ask-pass --ask-sudo-pass -vvvv
```
鍵を登録しているならask-passオプションは不要です
