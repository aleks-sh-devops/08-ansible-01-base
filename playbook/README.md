# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?
2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?
```
ansible-playbook -i ./inventory/test.yml site.yml
```
3. Какой командой можно зашифровать файл?
```
ansible-vault encrypt ./pass.yml

New Vault password:
Confirm New Vault password:
Encryption successful
```

4. Какой командой можно расшифровать файл?
```
ansible-vault decrypt ./pass.yml

```

5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?
```
ansible-vault view ./pass.yml

Ну и при редактировании тоже можно:
ansible-vault edit ./pass.yml
```

6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?
```
ansible-playbook -I inventory/hosts.yml site.yml --ask-vault-pass
```

8. Как называется модуль подключения к host на windows?
9. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh
10. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?
