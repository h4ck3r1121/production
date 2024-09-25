# Установка дополнительного ПО для production
1. Открыть файл "hosts" и прописать IP-адрес сервера, и, если нужно, имя пользователя и путь к private-ключу. Если private-ключа нет, то обратиться к главному системному администратору или руководителю проекта.
2. В файле "install-template-service.yml" в переменной docker_image прописать нужный docker-образ, если нужно, а также раскомментировать нижнюю строку, если нужно активировать автозагрузку сервиса.
3. Запустить "install-template-service.yml" с ключом "-b".

P.S.: если не хватает дополнительного ПО, то нужно запустить данный [playbook](https://github.com/h4ck3r1121/infrastructure-for-testing/blob/infra/install-needed-software.yml)