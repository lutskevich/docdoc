# docdoc
test role for docdoc

Имеем папку, в которой лежат файлы, имена файлов - это имена
пользователей. Нужно: написать ansible плейбук, который по имени
каждого файла в этой папке, будет создавать пользователя на сервере и
давать пользователю судо права на команду /opt/script.sh и запретит
вход по ssh(например для запуска команды через cron) , В конце плейбук
отправит письмо со списком всех добавленных пользователей.

docdoc_mailhost: smtp.gmail.com                                 # default mail server
docdoc_mailpassword: 8HD6PR2M                                   # ansible mail password 
docdoc_mailport: 587                                            # smtp port
docdoc_mailreceiver: lutskevich68@gmail.com                     # admin's mail
docdoc_mailusername: docdoctest7899@gmail.com                   # ansible mail address
docdoc_userpassword: $6$rounds=656000$DocDoc$C5UtYBsBJEPyjx6H0SgFn8.x2UEZnKXByEEsXq3VCP9AyTPu5xWVB7BuJFUSvnBPI/8FCsnnIXrqZx4MPUzSv0                                     # users default password (Qwe12345)
docdoc_userpath: /etc/users                                     # path to files with usernames
