### Описание проекта
Заказчик этого исследования — сеть отелей «Как в гостях». <p>
Чтобы привлечь клиентов, эта сеть отелей добавила на свой сайт возможность забронировать номер без предоплаты. Однако если клиент отменял бронирование, то компания терпела убытки. Сотрудники отеля могли, например, закупить продукты к приезду гостя или просто не успеть найти другого клиента.<p>
Чтобы решить эту проблему, вам нужно разработать систему, которая предсказывает отказ от брони. Если модель покажет, что бронь будет отменена, то клиенту предлагается внести депозит. Размер депозита — 80% от стоимости номера за одни сутки и затрат на разовую уборку. Деньги будут списаны со счёта клиента, если он всё же отменит бронь.<p>
### Бизнес-метрика и другие данные<p>
Основная бизнес-метрика для любой сети отелей — её прибыль. Прибыль отеля — это разница между стоимостью номера за все ночи и затраты на обслуживание: как при подготовке номера, так и при проживании постояльца. <p>
В отеле есть несколько типов номеров. В зависимости от типа номера назначается стоимость за одну ночь. Есть также затраты на уборку. Если клиент снял номер надолго, то убираются каждые два дня. <p>
Стоимость номеров отеля:<p>
категория A: за ночь — 1 000, разовое обслуживание — 400;<p>
категория B: за ночь — 800, разовое обслуживание — 350;<p>
категория C: за ночь — 600, разовое обслуживание — 350;<p>
категория D: за ночь — 550, разовое обслуживание — 150;<p>
категория E: за ночь — 500, разовое обслуживание — 150;<p>
категория F: за ночь — 450, разовое обслуживание — 150;<p>
категория G: за ночь — 350, разовое обслуживание — 150.<p>
В ценовой политике отеля используются сезонные коэффициенты: весной и осенью цены повышаются на 20%, летом — на 40%.<p>
Убытки отеля в случае отмены брони номера — это стоимость одной уборки и одной ночи с учётом сезонного коэффициента.<p>
На разработку системы прогнозирования заложен бюджет — 400 000. При этом необходимо учесть, что внедрение модели должно окупиться за тестовый период. Затраты на разработку должны быть меньше той выручки, которую система принесёт компании.<p>
### Оформление
Выполните задание в Jupyter Notebook. Заполните программный код в ячейках типа code, текстовые пояснения — в ячейках типа markdown. Используйте форматирование и заголовки.<p>
### Описание данных
В таблицах hotel_train и hotel_test содержатся одинаковые столбцы:<p>
id — номер записи;<p>
adults — количество взрослых постояльцев;<p>
arrival_date_year — год заезда;<p>
arrival_date_month — месяц заезда;<p>
arrival_date_week_number — неделя заезда;<p>
arrival_date_day_of_month — день заезда;<p>
babies — количество младенцев;<p>
booking_changes — количество изменений параметров заказа;<p>
children — количество детей от 3 до 14 лет;<p>
country — гражданство постояльца;<p>
customer_type — тип заказчика:<p>
Contract — договор с юридическим лицом;<p>
Group — групповой заезд;<p>
Transient — не связано с договором или групповым заездом;<p>
Transient-party — не связано с договором или групповым заездом, но связано с бронированием типа Transient.<p>
days_in_waiting_list — сколько дней заказ ожидал подтверждения;<p>
distribution_channel — канал дистрибуции заказа;<p>
is_canceled — отмена заказа;<p>
is_repeated_guest — признак того, что гость бронирует номер второй раз;<p>
lead_time — количество дней между датой бронирования и датой прибытия;<p>
meal — опции заказа:<p>
SC — нет дополнительных опций;<p>
BB — включён завтрак;<p>
HB — включён завтрак и обед;<p>
FB — включён завтрак, обед и ужин.<p>
previous_bookings_not_canceled — количество подтверждённых заказов у клиента;<p>
previous_cancellations — количество отменённых заказов у клиента;<p>
required_car_parking_spaces — необходимость места для автомобиля;<p>
reserved_room_type — тип забронированной комнаты;<p>
stays_in_weekend_nights — количество ночей в выходные дни;<p>
stays_in_week_nights — количество ночей в будние дни;<p>
total_nights — общее количество ночей;<p>
total_of_special_requests — количество специальных отметок.<p>
