Домашнее задание к занятию 10.4 «Резервное копирование»

Инструкция по выполнению домашнего задания

Сделайте fork репозитория c Шаблоном решения к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/gitlab-hw или https://github.com/имя-вашего-репозитория/8-03-hw).

Выполните клонирование данного репозитория к себе на ПК с помощью команды git clone.

Выполните домашнее задание и заполните у себя локально этот файл README.md:
впишите вверху название занятия и вашу фамилию и имя
в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
для корректного добавления скриншотов воспользуйтесь инструкцией "Как вставить скриншот в шаблон с решением"
при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в инструкции по MarkDown)

После завершения работы над домашним заданием сделайте коммит (git commit -m "comment") и отправьте его на Github (git push origin);

Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.

Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.

Желаем успехов в выполнении домашнего задания!



Задание 1

В чём разница между:

полным резервным копированием,
дифференциальным резервным копированием,
инкрементным резервным копированием.

Приведите ответ в свободной форме.

Ответ: 

Дифференциальное – это такое резервное копирование, при котором полная копия создаётся единожды в начале, а все последующие копии, создаваемые в рамках одной и той же задачи, содержат не все данные, а лишь произошедшие изменения с момента создания первичной полной копии. Ключевой момент здесь – с момента создания полной копии.

Инкрементное копирование (Incremental Backup) — это метод сохранения информации, при котором архивируются только измененные с момента последнего бэкапа данные. Каждая последующая операция по резервированию добавляет на носитель новые или измененные файлы без замены старых. Этим достигается более высокая скорость копирования, чем при процедуре полного или дифференциального копирования.

Полное – это резервное копирование, при котором снимок операционной системы, диска, раздела или отдельных папок содержит все резервируемые данные. Такие снимки, создаваемые в рамках одной и той же задачи по бэкапу, независимы друг от друга, повреждение одного из них никак не повлияет на другие снимки.



Задание 2

Установите программное обеспечении Bacula, настройте bacula-dir, bacula-sd, bacula-fd. Протестируйте работу сервисов.

Пришлите:

- конфигурационные файлы для bacula-dir, bacula-sd, bacula-fd,
- скриншот, подтверждающий успешное прохождение резервного копирования.

Ответ: 




