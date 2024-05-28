# task3

## Я решила создать мобильное приложение YumExpress. 

Что это такое? 

Это мобильное приложение для заказа еды из ресторанов с доставкой на дом или на работу. Приложение нужно, чтобы упростить процесс заказа еды и сделать его максимально комфортным  для использования заказчиков и ресторанов. 

## Функции приложения: 

### Для пользователей: 

Просмотр меню: Клиенты могут увидеть меню из разных ресторанов с изображениями.

Поиск и фильтры: Возможность быстро и удобно найти желаемое блюдо или ресторан (выбор кухни, стоимости, рейтинга и другое). 

Оформление заказа: Добавление и удаление блюд из корзины, выбор способа оплаты (онлайн или наличными), указание адреса и времени доставки. 

Отслеживание заказа: Пользователи могут в режиме реального времени видеть статус своего заказа: подтвержден, готовится, передано, доставлен. 

Отзывы: Возможность оценивать рестораны и оставлять отзывы о качестве блюд и сервиса. 

История заказов: Просмотр истории своих заказов с возможностью повторить заказ в один клик. 

Поддержка: Онлайн-чат с оператором для решения любых вопросов, связанных с заказом. 

### Для ресторанов: 

Личный кабинет: Управление меню, добавление новых блюд, изменение цен, установка графика работы. 

Прием заказов: Получение уведомлений о новых заказах, возможность подтверждать или отклонять заказы. 

Статистика и аналитика: Отслеживание ключевых показателей, таких как количество заказов, средний чек, популярные блюда. 

Интеграция с POS-системой: Возможность интеграции с системой учета товаров и продаж ресторана. 

### Для курьеров: 

Регистрация в системе: Курьеры могут зарегистрироваться в приложении, указав свои данные и зону доставки. 

Получение заказов: Курьеры получают уведомления о новых заказах, находящихся в их зоне доставки. 

Карта доставки: Курьеры видят на карте оптимальный маршрут до ресторана и адреса доставки.

Статус доставки: Курьеры могут менять статус доставки (взят в работу, в пути, доставлен).

### В будущес YumExpress будет стремится стать незаменимым помощником для всех, кто ценит свое время и любит вкусную еду.

Диаграмму вариантов использования: 
1.  Заказать еду:Пользователь просматривает меню, добавляет блюда в корзину, оформляет заказ с указанием адреса и времени доставки.
2.  Управлять меню:Ресторан добавляет новые блюда, редактирует меню, устанавливает цены.
3.  Принять/отклонить заказ:Ресторан получает уведомление о новом заказе и может подтвердить или отклонить его. 
4.  Доставить заказ:Курьер получает информацию о заказе, забирает его из ресторана и доставляет пользователю.
5.  Отслеживать заказ:Пользователь и ресторан могут отслеживать статус заказа в реальном времени.

Пользователь может "Заказать еду" и "Отслеживать заказ".
Ресторан может "Управлять меню", "Принять/отклонить заказ" и "Отслеживать заказ".
Курьер может "Доставить заказ".

Данная диаграмма отображает только основные варианты использования. Дополнительные функции, такие как оплата, отзывы, история заказов и т.д., могут быть добавлены в виде отдельных use cases  при необходимости.

![Иллюстрация к проекту](https://github.com/remafka/task3/blob/c00d699cd979836fd6db7aae4605041d593b55fd/%D0%94%D0%B8%D0%B0%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D1%83%20%D0%B2%D0%B0%D1%80%D0%B8%D0%B0%D0%BD%D1%82%D0%BE%D0%B2%20%D0%B8%D1%81%D0%BF%D0%BE%D0%BB%D1%8C%D0%B7%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F.png)


Диаграмму последовательности для процесса заказа еды через приложение

Описание:

1. Пользовательоткрывает приложение FoodExи выбирает ресторан и нужные блюда.
2. Приложениеотправляет запрос на Сервердля получения меню выбранного ресторана.
3. Сервервозвращает меню ресторана в Приложение.
4. Пользовательдобавляет выбранные блюда в корзину.
5. Пользовательпереходит к оформлению заказа.
6. Пользовательуказывает адрес и время доставки, выбирает способ оплаты. 
7. Приложениеотправляет данные о заказе на Сервер.
8. Серверпередает заказ в выбранный Ресторан.
9. Ресторанможет подтвердить или отклонить заказ.
10. Серверполучает ответ от Ресторанаи передает его в Приложение.
11. Приложениеотображает Пользователюстатус заказа ("Подтвержден" или "Отклонен").

Примечание:

Данная диаграмма последовательности описывает только процесс оформления и подтверждения заказа. Последующие этапы, такие как приготовление, передача заказа курьеру, доставка и оплата, могут быть представлены на отдельных диаграммах для более детального описания процесса. 

Диаграмму состояний для заказа
Описание состояний:

Новый:Заказ только что создан пользователем и ожидает подтверждения рестораном.
Подтвержден:Ресторан подтвердил заказ и начал его обработку.
Готовится:Заказ находится в процессе приготовления на кухне ресторана.
Передан курьеру:Заказ приготовлен и передан курьеру для доставки.
Доставлен:Курьер доставил заказ пользователю.
Отменен:Заказ был отменен пользователем или рестораном, либо возникли проблемы с доставкой.

Описание переходов:

Ресторан подтвердил:Переход из состояния "Новый" в состояние "Подтвержден", когда ресторан подтверждает заказ.
Ресторан отклонил / Пользователь отменил:Переход из состояния "Новый" в состояние "Отменен", если ресторан отклонил заказ или пользователь отменил его до подтверждения рестораном.
Ресторан начал готовить:Переход из состояния "Подтвержден" в состояние "Готовится", когда ресторан начинает готовить заказ.
Курьер забрал заказ:Переход из состояния "Готовится" в состояние "Передан курьеру", когда курьер забирает заказ из ресторана.
Курьер доставил заказ:Переход из состояния "Передан курьеру" в состояние "Доставлен", когда курьер доставляет заказ пользователю.
Проблемы с доставкой / Пользователь отменил:Переход из состояния "Передан курьеру" в состояние "Отменен", если возникли проблемы с доставкой или пользователь отменил заказ после его передачи курьеру.

Примечание:

Это упрощенная диаграмма состояний. В реальном приложении могут быть дополнительные статусы и переходы, например: 
"Ожидает оплаты" (если выбран онлайн-платеж)
"Ожидает подтверждения оплаты" 
"Возврат средств" (если заказ отменен и требуется возврат) 

 Конкретные статусы и переходы будут зависеть от требований к приложению FoodEx.



 Диаграмму деятельности для описания процесса обработки заказа системой

 Описание:

1. Пользователь оформляет заказ:Процесс начинается с того, что пользователь формирует заказ в приложении, выбирая блюда и указывая информацию для доставки.
2. Проверка наличия блюд:Система проверяет, доступны ли выбранные блюда в ресторане.
    Если все блюда доступны:Процесс продолжается.
    Если есть недоступные блюда:Пользователь получает уведомление и может скорректировать заказ.
3. Создание и отправка заказа:Система создает новый заказ и отправляет его в ресторан. 
4. Ресторан получает и обрабатывает заказ:Ресторан получает уведомление о новом заказе.
    Ресторан подтверждает заказ:Система ищет доступных курьеров.
        Курьер найден:Система назначает курьера на заказ, и он получает уведомление. Курьер принимает заказ, забирает его из ресторана и доставляет пользователю. Система уведомляет пользователя о каждом этапе доставки. После получения заказа, пользователь может оценить его.
        Курьер не найден:Система уведомляет пользователя о возможном долгом ожидании курьера.
    Ресторан отклоняет заказ:Система уведомляет пользователя об отклонении заказа.

Примечание:

Данная диаграмма деятельности представляет общий сценарий обработки заказа. В реальности могут быть дополнительные шаги и условия, например: 

Проверка и обработка онлайн-оплаты.
Обработка отмены заказа пользователем или курьером.
Обработка возникающих проблем во время доставки.
Интеграция с POS-системой ресторана. 



Диаграмму классов для системы. 

Описание:

Диаграмма классов демонстрирует основные классы (или "модули") системы FoodEx и их взаимосвязи:

Пользовательское приложение:
Пользователь: класс, представляющий пользователя системы. 
Меню:отвечает за отображение меню ресторанов и блюд.
Заказ:хранит информацию о заказе.

Система FoodEx:
Модуль авторизации:отвечает за регистрацию и вход пользователей.
Модуль меню: управляет меню ресторанов и отображает его пользователям.
Модуль заказов: обрабатывает заказы, отслеживает их статусы и хранит историю заказов.
Модуль оплаты: обрабатывает онлайн и оффлайн платежи.
Модуль доставки:назначает курьеров, отслеживает их местоположение и рассчитывает время доставки.
Модуль поддержки:предоставляет пользователям доступ к онлайн-чату и FAQ.

Приложение ресторана:
Ресторан: класс, представляющий ресторан. 

Приложение курьера:
Курьер: класс, представляющий курьера.


Взаимодействие между классами:

Пользователи взаимодействуют с системой через Пользовательское приложение, оформляют заказы, отслеживают их статусы, и т.д.
Система FoodEx обрабатывает заказы, взаимодействует с ресторанами и курьерами.
Рестораны получают заказы, подтверждают их, готовят еду и передают ее курьерам.
Курьеры принимают заказы, забирают их из ресторанов и доставляют пользователям. 


Примечание:

Это упрощенная диаграмма классов. В реальной системе FoodEx будет значительно больше классов и связей между ними. Детализация диаграммы зависит от конкретных требований к системе.
.
