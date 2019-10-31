### Реализовать knocking port. centralRouter может попасть на ssh inetrRouter через knock скрипт.

Проверка:

vagrant ssh centralRouter

for i in 8881 7777 9991; do sudo nmap -Pn --host_timeout 100 --max-retries 0 -p $i 192.168.255.1; done

ssh vagrant@192.168.255.1 [пароль: vagrant]

### Запустить nginx на centralServer, пробросить 80й порт на inetRouter2 8080

После запуска  стенда из Vagrantfile на хоствой машине необходимо перейти на http://127.0.0.1:8080, где будет доступна стандартная страница nginx.
