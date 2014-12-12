# Словарь понятий



<a id="BitPie.NET"></a>__BitPie.NET__
:   глобальная сеть для распределенного хранения и обмена данными
  
<a id="Программа"></a>__Программа BitPie.NET__
:   программное обеспечение с открытым (доступным для свободного скачивания и просмотра) исходным кодом, 
    предоставляемое и распространяемое [BitPie.NET Inc.](http://bitpie.net) под данной 
    [лицензией](http://bitpie.net/license.html)  
  
<a id="Узел"></a>__Узел__
:   компьютер, подключенный к сети интернет, на котором установлено [ПО BitPie.NET](#Программа)  

<a id="Сеть"></a>__Сеть BitPie.NET__
:   добровольное объединение людей, использующих свои личные компьютеры как
    отдельные взаимодействующие друг с другом [узлы BitPie.NET](#Узел)  

<a id="Данные"></a>__Данные__
:   любая информация, которую можно хранить в виде файла на жестком диске компьютера



<a id="Копия"></a>__Резервная копия__
:   точная копия определенных [данных](#Данные), созданная в некий момент времени



<a id="Резервная копия папки"></a>__Резервная копия папки__
:   это [резервная копия](#Копия) данных, полученных архивированием всех файлов, 
    хранящихся в данной папке на жестком диске компьютера, 
    включая (по выбору пользователя) и все подпапки



<a id="Распределенная копия"></a>Распределенная копия__
:   это [резервная копия](#Резервная копия), которая хранится 
    на различных [узлах](#Узел) в [сети BitPie.NET](#Сеть)



<a id="Хранение данных в сети BitPie.NET"></a>__Хранение данных__
:   методика обработки информации при которой исходные данные:

    + [шифруются](#Шифрование),
    + [архивируются](#Архивация)
    + и размещаются на разных [узлах](#Узел), разбитые на [блоки](#Блок) и [куски](#Кусок)  
  
<a id="Блок"></a>__Блок__
:   файл на жестком диске содержащий лишь часть [резервной копии](#Копия) и
    имеющий порядковый номер, присваиваемый в момент создания блока



<a id="Кусок"></a>__Кусок__
:   часть [блока](#Блок), полученная в процессе создания [резервной копии](#Копия) и
    имеющая порядковый номер - позицию в блоке


    
<a id="Пакет"></a>__Пакет__ или __Служебный пакет__
:   полезная информация, передаваемая от одного [узла](#Узел) к другому в [сети BitPie.NET](#Сеть)
    и содержащая электронную подпись отправителя



<a id="Пакет данных"></a>__Пакет данных__ или __Порция данных__
:   это [пакет], который содержит [зашифрованный](#Шифрование) [кусок](#Кусок) [данных](#Данные)



<a id="Восстановление"></a>__Восстановление__
:   процесс обратного преобразования [данных](#Данные) из отдельных [кусков](#Кусков) и
    воссоздания исходной информации из [Резервной копии](#Копия)



<a id="Хранитель"></a>__Хранитель__
:   [узел](#Узел) в [сети BitPie.NET](#Сеть), чей владелец добровольно согласился хранить [данные](#Данные) 
    других пользователей на жестком диске своего персонального компьютера



<a id="Клиент"></a>__Клиент__
:   [узел](#Узел) в [сети BitPie.NET](#Сеть), владелец которого использует пространство на жестком диске
    других [узлов](#Узел) для хранения своих [данных](#Данные)



<a id="Donated folder"></a>__Donated folder__
:   папка на жестком диске [пользователя](#пользователя), где хранятся [данные](#Данные) его [Customer](#Customer)'ов



<a id="Donated space"></a>__Donated space__
:   максимальный размер который может иметь [Donated folder](#Donated folder)



<a id="Used Donated space"></a>__Used Donated space__
:   текущий размер [Donated folder](#Donated folder)



<a id="Free Donated space"></a>__Free Donated space__
:   разность между [Donated space](#Donated space) и [Used Donated space](#Used Donated space)



<a id="Backup size"></a>__Backup size__
:   суммарный размер всех [блоков](#блоков) относящихся к данному [Backup](#Backup)'у



<a id="Used space"></a>__Used space__
:   суммарный размер всех уже созданных [Backup](#Backup)'ов данного [пользователя](#пользователя)



<a id="Needed space"></a>__Needed space__
:   верхняя граница [Used space](#Used space) для данного [пользователя](#пользователя)



<a id="Free space"></a>__Free space__
:   разность между [Needed space](#Needed space) и [Used space](#Used space)



<a id="Команда"></a>__Команда__
:   [пакет](#пакет) [данных](#данных) содержащий лишь короткую кодовую фразу, [сообщение](#сообщение) или другие [данные](#Данные) и используемый для взаимодействия [пользователей](#пользователей)



<a id="Сообщение"></a>__Сообщение__
:   текстовое сообщение адресованное конкретному [пользователю](#пользователю)



<a id="Модуль"></a>__Модуль__
:   отдельная часть программного кода входящая в состав [BitPie.NET Software](#BitPie.NET Software)



<a id="Транспорт"></a>__Транспорт__
:   [модуль](#модуль) осуществляющий передачу и прием [пакетов](#пакетов) по определенному [протоколу](#протоколу)



<a id="Протокол"></a>__Протокол__
:   правило описывающее способ передачи информации между компьютерами



<a id="Контакт"></a>__Контакт__
:   строка вида [протокол]://[адрес], уникальная для всякого [пользователя](#пользователя)



<a id="Шифрование"></a>__Шифрование__
:   преобразование [данных](#данных) с целью их защиты



<a id="Архивация"></a>__Архивация__
:   преобразование [данных](#данных) с целью уменьшения их размера



<a id="Открытый ключ"></a>__Открытый ключ__, 
<a id="Закрытый ключ"></a>__Закрытый ключ__ и 
<a id="Цифровая подпись"></a>__Цифровая подпись__
:   смотреть <a href="http://ru.wikipedia.org/wiki/%D0%9A%D1%80%D0%B8%D0%BF%D1%82%D0%BE%D1%81%D0%B8%D1%81%D1%82%D0%B5%D0%BC%D0%B0_%D1%81_%D0%BE%D1%82%D0%BA%D1%80%D1%8B%D1%82%D1%8B%D0%BC_%D0%BA%D0%BB%D1%8E%D1%87%D0%BE%D0%BC">статью на википедии</a>.



<a id="Identity"></a>__Identity__
:   общедоступный файл содержащий [открытый ключ](#открытый ключ), [цифровую подпись](#цифровую подпись), [контакты](#контакты) и другую информацию относящуюся к определенному  [пользователю](#пользователю)



<a id="Identity сервер"></a>__Identity сервер__
:   сервер регистрирующий и хранящий файлы [Identity](#Identity)



<a id="Identity URL"></a>__Identity URL__ или 
<a id="IDURL"></a>__IDURL__
:   адрес файла [Identity](#Identity) в интернете



<a id="Центральный сервер"></a>__Центральный сервер__
:   [пользователь](#пользователь) ответственный за [регистрацию](#регистрацию) и [обслуживание](#обслуживание) всех остальных [пользователей](#пользователей) системы



<a id="Регистрация пользователя"></a>__Регистрация пользователя__
:   процесс создания нового файла [Identity](#Identity) на [сервере Identity](#сервере Identity) и новой [учетной записи](#учетной записи) на [Центральном сервере](#Центральном сервере)



<a id="Учетная запись"></a>__Учетная запись__
:   совокупность [данных](#данных) на [Цетральном сервере](#Цетральном сервере) относящихся к данному [пользователю](#пользователю)



<a id="Обслуживание пользователя"></a>__Обслуживание пользователя__
:   набор функций предоставляемых [Центральным сервером](#Центральным сервером) основная из которых подбор [Supplier](#Supplier)'ов для [пользователей](#пользователей)



<a id="Money сервер"></a>__Money сервер__
:   [пользователь](#пользователь) осуществляющий ввод и вывод денежных средств



<a id="Receipt"></a>__Receipt__
:   [сообщение](#сообщение) содержащее отчет о перемещении денежных средств



<a id="Recovery"></a>__Recovery__
:   процесс восстановления [учетной записи](#учетной записи) [пользователя](#пользователя) по [IDURL](#IDURL) и [закрытому ключу](#закрытому ключу)
 