---
order: 500
icon: file
---

# СRM - подсистема

!!!
**CRM система управления взаимоотношениями с клиентами** - модель взаимодействия, основанная на теории, что центром всей философии бизнеса является клиент, а главными направлениями деятельности компании являются меры по обеспечению эффективного маркетинга, продаж и обслуживания клиентов. Поддержка этих бизнес-целей включает сбор, хранение и анализ информации о потребителях, поставщиках, партнёрах, а также о внутренних процессах компании. Функции для поддержки этих бизнес-целей включают продажи, маркетинг, поддержку потребителей.
!!!

В нашей конфигурации предусмотрена подсистема "CRM". Работа данного функционала схожа с работой подсистемы "Техническая поддержка". Инциденты, поступившие в Service Desk, поэтапно обрабатываются специалистами и доводятся до логического завершения. В CRM все обстоит точно также, чтобы в этом убедиться схематично рассмотрим работу подсистемы:

![01_CRM](static/01_CRM.png)

Что мы видим? Как и у системы обработки инцидентов, цель CRM аналогична, довести обращение до завершения, а именно, это потенциального клиента перевести в статус клиента. Следовательно, механизм технической поддержки полностью подходит для создания ЦРМ, за исключением добавления в работу новой сущности ["Потенциальные клиенты"](https://softonit.ru/FAQ/courses/?COURSE_ID=1&LESSON_ID=635&LESSON_PATH=1.22.634.635). Разберем настройку, на примере.

Первым делом, что необходимо сделать - это создать **процесс** и настроить его **этапы**, по которым будем работать с обращениями потенциальных клиентов. Перейдем в **("Справочники"->"Service Desk"->"Процессы")** и создадим новый процесс "Проявление интереса".

![02_CRM](static/02_CRM.png)

Согласно схеме, представленной выше, настроим этапы процесса следующим образом:
* **Новый** - новое обращение (возможен переход на этапы "Выбор", "Отказ").
* **Выбор** - потенциальный клиент стоит перед выбором продолжения взаимоотношений (возможен переход на этапы "Выставление счета", "Отказ").
* **Выставление счет**а - потенциальный клиент продолжил взаимоотношения и ожидает счета на оплату (возможен переход на этапы "Оплачен", "Отказ").
* **Оплачен** - счет оплачен (возможен переход на этап "Ожидание документов").
* **Ожидание документов** - ожидаем закрывающих документов (возможен переход на этап "Клиент").
* **Клиент** - потенциальный клиент переведен в статус клиента (возможен переход на этап "Работа по договору").
* **Работа по договору**  - работаем с клиентом по заключенному договору (возможен переход на этап "Выставление счета" в случае истечения срока действия заключенного договора).
* **Отказ** - клиент отказался вести взаимоотношения на этапах ("Новый", "Выбор", "Выставление счета").

![03_CRM](static/03_CRM.png)

После переходим к созданию новой учетной записи, на которую будем получать обращения потенциальных клиентов **("Администрирование" -> "Учетные записи электронной почты")**. Стоит заметить, что при использовании подсистемы "CRM" необходимо иметь минимум две учетные записи. Одну использовать для создания заданий на основе инцидентов, а другую для работы с "CRM".

![04_CRM](static/04_CRM.png)

Следующий шаг, это настройка правил событий. Перейдем в *("Справочники" -> "Правила событий")* и создадим/скопируем правило событий "Электронное письмо входящее (запись)" для создания заданий(обращений) на основе входящей электронной почты. 

![05_CRM](static/05_CRM.png)

Заполним реквизиты и добавим новый элемент отбора (**"Учетная запись" = "CRM"**), таким образом при получении почты на почтовый адрес, указанный в данной учетной записи, будет отрабатывать действие к настройке, которого перейдем далее.

![06_CRM](static/06_CRM.png)

Скопируем действие правил событий, которое используется для создания заданий на основании почтовых обращений и изменим его. На закладке "Значения заполнения" изменим реквизиты в соответствии с рисунком выше. Очень важный реквизит в данном случае "процесс", созданный нами ранее и в соответствии, с которым далее будет разделение на "инциденты" и "проявленный интерес" потенциальных клиентов.
На закладке "Инициаторы" необходимо выставить приоритет поиска инициаторов при записи входящего письма. 

![07_CRM](static/07_CRM.png)

Обратите внимание, что сущность "Потенциальные клиенты" находится вверху списка, а также выбрана в поле "Создавать инициатора с типом, если он не найден". При таких настройках после создания задания, потенциальные клиенты будут добавлены в одноименный справочник. 

![08_CRM](static/08_CRM.png)

Для более удобной работы с подсистемой "CRM" можно использовать "Канбан-доску".  Перейдем в *("Техническая поддержка" -> "Группы канбан-доски")* и добавим новые группы, которые будут отображаться на канбан. 

![09_CRM](static/09_CRM.png)

При создании группы, важно не забывать выставлять реквизит "Отображать" в положение "Да" иначе на канбан-доске она не будет отображаться.

![10_CRM](static/10_CRM.png)

После этого создаем новую канбан-доску и добавляем группы, которые создали ранее.

![11_CRM](static/11_CRM.png)

Результат канбан-доски "CRM".

![12_CRM](static/12_CRM.png)

Итог настройки подсистемы.
В документе "Задания" будут созданы задания на основании обращений потенциальных клиентов, поступивших на почту "CRM". Действием правил событий автоматически проставляются реквизиты задания. В справочник "[Потенциальные клиенты](https://softonit.ru/FAQ/courses/?COURSE_ID=1&LESSON_ID=635&LESSON_PATH=1.22.634.635)" добавляется новая позиция и после чего можно приступить к работе с потенциальным клиентом.

![13_CRM](static/13_CRM.png)

Сортировкой по процессам, можно отделить инциденты от проявленных интересов.

![14_CRM](static/14_CRM.png)


**Список ролей для работы с подсистемой "CRM".**
* [x] Выполнение заданий;
* [x] Добавление заданий; 
* [x] Добавление изменение спринтов;   
* [x] Оценка заданий из электронных писем;   
* [x] Просмотр не распределенных заданий;   
* [x] Просмотр отчетов по заданиям;   
* [x] Просмотр чужих заданий;    
* [x] Распределение заданий;   
* [x] Управление процесxсами и этапами;   
* [x] Чтение заданий.  









