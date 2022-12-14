# TRITPO_lab4
### Содержание
  1. [Введение](#1)
  2. [Объект тестирования](#2)
  3. [Атрибуты качества](#3)
  4. [Риски](#4)
  5. [Аспекты тестирования](#5)<br>
    5.1. [Возможность создания напоминания](#001)<br>
    5.2. [Возможность удаления напоминания](#002)<br>
    5.3. [Возможность редактирования напоминания](#003)<br>
    5.4. [Возможность настройки приложения](#004)<br>
    5.5. [Возможность просмотра списка всех напоминаний](#005)<br>
    5.6. [Изменение просмотра профиля](#006)<br>
6. [Подходы к тестированию](#6)
7. [Представление результатов](#7)
8. [Выводы](#8)


<a name="1"></a>
### 1. Введение
Данный план предназначен для тестирования приложения "RemindMe". Цель проведения тестирования - проверка работоспособности и пригодности приложения для практического использования.
В данном плане используется терминология, соответствующая данному приложению, просьба перед его прочтением ознакомится с [глоссарием приложения "RemindMe"](https://github.com/Dufal/TRITPO_lab3/blob/main/Glossary.md)

<a name="2"></a>
### 2. Объект тестирования
В качестве объектов тестирования можно выделить атрибуты качества платформы по ISO 25010:
1. функциональность
	- функциональная полнота: приложение должно выполнять все заявленные функции
	- функциональная корректность: приложение должно выполнять все заявленные функции корректно
	- функциональная целесообразность: отсутствуют не заявленные функции, которые бы мешали приложению выполнять первоначально поставленные задачи
2. удобство использования
	- эстетика пользовательского интерфейса: элементы управления объектами должны быть всегда доступны пользователю
	- защищённость от ошибки пользователя: запрос подтверждения пользователя при внесении им существенных изменений в объекты.

Данные атрибуты были взяты с учётом специфики приложения.

Тестируемое приложение содержит 1 модуль, созданный для выполнения определённого функционала:
 - главное окно (окно управления приложением).


<a name="3"></a>
### 3. Атрибуты качества
1. Функциональность:
    - функциональная полнота: приложение должно соответствовать всем функциональным требованиям, заявленных в [TECHNICAL SPECIFICATION](https://github.com/Dufal/TRITPO_lab2/blob/main/TECHNICAL%20SPECIFICATION.md);
    - функциональная целесообразность: отсутствуют не заявленные функции, которые бы мешали приложению выполнять поставленные задачи
2. Удобство использования:
    - простота пользовательского интерфейса: интерфейс должен быть достаточно простым для интуитивного использования новым пользователем.
3. Кроссплатформенность:
    - корректная работа приложения на платформах:
      - Windows
      - Linux.

<a name="4"></a>
### 4. Риски
Приложение использует системные средства для отображения текста, из-за чего представление некоторых символов на разных операционных системах может отличаться. 


<a name="5"></a>
### 5. Аспекты тестирования
Данное тестирование является интеграционным, т. е. программные модули тестируются в группке, также является дымовым, и будет проводиться по типу "Black box", т. е. без доступа к исходному коду.<br>
В ходе тестирования планируется проверить реализацию основных функций приложения, провести позитивные и негативные тесты, а также проверить нефункциональные требования. К основным функциям можно отнести следующие пункты:

- возможность создания напоминания;
- возможность удаления напоминания;
- возможность редактирования напоминания:
- возможность настройки приложения;
- возможность просмотра списка всех напоминаний;
- возможность просмотра профиля;


#### Функциональные требования:

<a name="001"></a>
##### Возможность создания напоминания
Этот вариант использования небходимо протестировать на:
1. Реакцию приложения на попытку создания напоминания.
2. Выполнение данной операции (действительное создание напоминания при нажатии кнопки).

<a name="002"></a>
##### Возможность удаления напоминания
Этот вариант использования небходимо протестировать на:
1. Реакцию приложения на попытку удалить напоминания.
2. Выполнение данной операции (действительное удаление напоминания при нажатии кнопки).

<a name="003"></a>
##### Возможность редактирования напоминания
Этот вариант использования небходимо протестировать на:
1. Реакцию приложения на редактирование напоминания.
2. Выполнение данной операции (действительное редактирование напоминания при нажатии кнопки).

<a name="004"></a>
##### Возможность настройки приложения
Этот вариант использования небходимо протестировать на:
1. Реакцию приложения на попытку настройки приложения.
2. Выполнение данной операции (настройка приложения)

<a name="005"></a>
##### Возможность просмотра списка всех напоминаний
Этот вариант использования небходимо протестировать на:
1. Реакцию приложения на попытку просмотра списка всех напоминаний.
2. Выполнение данной операции (просмотр списка).

<a name="006"></a>
##### Возможность просмотра профиля
Этот вариант использования небходимо протестировать на:
1. Реакцию приложения на просмотреть профиль.
2. Выполнение данной операции (действительный просмотр профиля).


#### Нефункциональные требования:
- быстрый запуск приложения;
- все элементы пользовательского интерфейса имеют название, описывающее действие которое они выполняют.

<a name="6"></a>
### 6. Подходы к тестированию
Проводимое тестирование можно опередлить как:
  - По степени автоматизации: ручное.
  - По знанию системы: черный ящик.
  - По степени изолированности компонентов: интеграционное.

<a name="7"></a>
### 7. Представление результатов
Результаты тестирования представлены в [таблице](https://github.com/Dufal/TRITPO_lab4/blob/main/TestResult.md).

<a name="8"></a>
### 8. Выводы
Данный тестовый план позволяет протестировать основной функционал приложения. Успешное прохождение всех тестов не гарантирует полной работоспособности на всех платформах и архитектурах, однако позволяет полагать, что данное программное обеспечение работает корректно.
