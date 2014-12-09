# Сервис customer()


## Описание
Сетевая служба `customer()` организует подключение пользователя к удаленным хранителям - узлам,
которые предоставляют свои жесткие диски для размещение личных данных пользователя.

Сам пользователь является для этих узлов клиентом, поскольку арендует пространство на их жестких дисках.
В данный момент система монетизации распределенного хранения данных находится в стадии переработки и 
все пользователи предоставляют свое пространство в сеть BitPie.NET на добровольных основаниях.

Каждый участник сети BitPie.NET может выступать и как хранитель и как клиент.
Пользователь сможет разместить свои данные лишь на тех узлах, у которых
постоянно активна сетевая служба `supplier()`.

Для каждого хранителя будет создан экземпляр автомата `supplier_connector()`, он
производит подключение удаленному узлу и запрос дисковой квоты для хранения личных данных.

Подробнее о системе распределенного хранения данных в сети BitPie.NET чатайте в разделе [...](...).

При отключении сервиса `customer()` будет прекращено взаимодействие со всеми хранителями, что приведет
к полной потере всех сохраненных на данный момент данных.


## Зависит от
* [p2p_hookups()](services/service_p2p_hookups.md)


## Влияет на
* [data_sender()](services/service_data_sender.md)
* [fire_hire()](services/service_fire_hire.md)
* [list_files()](services/service_list_files.md)


## Запуск автоматов
* [supplier_connector()](customer/supplier_connector.md)


## Настройки сервиса
* services/customer/enabled - включение/выключение сервиса `customer()`
* services/customer/needed-space - общий объем запрошенного пользователем пространства под собственные данные 
* services/customer/suppliers-number - желаемое колличество хранителей


## Связанные файлы проекта
* [service/service_customer.py](services/service_customer.py)
* [customer/supplier_connector.py](customer/supplier_connector.py)
* [contacts/contactsdb.py](contacts/contactsdb.py)

