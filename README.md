# geonames-ua
Проєкт з оцифрування та уточнення географічних назв України з Державного реєстру географічних назв України https://land.gov.ua/derzhavnyi-reiestr-heohrafichnykh-nazv/

Державна служба України з питань геодезії, картографії та кадастру опублікувала у 2018 році дані з Державного реєстру географічних назв на підставі Закону України “Про географічні назви” та постанови Кабінету Міністрів України від 11 травня 2006 р. № 622 “Про затвердження Положення про Державний реєстр географічних назв”, наказу Мінагрополітики від 11.06.2014 № 219 «Про затвердження обліково-реєстраційних форм Державного реєстру географічних назв», зареєстрованого у Мін’юсті 24.06.2014 за № 683/25460.


_Але є одне але, ці дані у форматі PDF і їх точність через «округлення координат» є досить відносна. Я не є представником державних структур, просто зацікавлений волонтер, який вважає, що ці дані мають бути зручні для використання і за можливості максимально точні. Назви та розташування фізико-географічних об'єктів України чи об'єктів природно-заповідного фонду будуть корисні для природоохоронних організацій, OpenStreetMap маперів, туристів, краєзнавців, картографів та навіть у освітніх цілях для шкіл чи ЗВО та багатьох інших зацікавлених сторін._

#### Як оброблялись дані

PDF файли конвертувались у CSV за допомогою [Tabula](https://tabula.technology/). Потім виправлялись у LibreOffice та QGIS
Зараз вони «як є» з виправленням перевернутих координат та незначних помилок. Загалом дані __дуже не точні__ географічно, можливо через «округлення координат», але завдяки їм можливо створити відкриту базу геопросторових назв України. Дякуємо державній службі за відкритість, без цього не було б цих переліків.


#### Як користуватись

Ви можете вільно завантажувати ці дані. На сайті Державної служби України з питань геодезії, картографії та кадастру [land.gov.ua](https://land.gov.ua/)  увесь вміст доступний за ліцензією Creative Commons Attribution 4.0 International license, якщо не зазначено інше. Тож за такою ліцензією і розповсюджується і цей оцифрований матеріал.

Згодом тут будуть опубліковані дані у популярних картографічних форматах.

#### Як виправити помилки

За можливості, надсилайте виправлені некоректно розташовані координати точки у GeoJSON-файлі (наприклад: `"geometry": { "type": "Point", "coordinates": [ 31.xxxx, 48.xxxx ] }`), через [Pull requests](https://github.com/gontsa/geonames-ua/pulls). [Детальніше в документації GitHub](https://docs.github.com/en/github/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests). 

Таким чином зможемо актуалізувати базу геопросторових даних.


## Статус проєкту

* __Адміністративно-територіальні об'єкти України__ (В процесі)

* __Соціально-економічні об'єкти України__ (В процесі)

## Природно-заповідні об'єкти України

Дані опрацьовані та потребують верифікації.

| Регіон                    | Кількість об'єктів | GeoJSON | Статус |
|---------------------------|:---------:|:---:|:-------:|
| Вінницька область         |    285    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-vinnytska.geojson)   |         |
| Волинська область         |    286    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-volynska.geojson)   |         |
| Дніпропетровська область  |    88     |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-dnipropetrovska.geojson)   |         |
| Донецька область          |    94     |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-donetska.geojson)   |         |
| Житомирська область       |    161    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-zytomyrska.geojson)   |         |
| Закарпатська область      |    76     |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-zakarpatska.geojson)   |         |
| Запорізька область        |    284    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-zaporizska.geojson)   |         |
| Івано-Франківська область |    330    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-ivano-frankivska.geojson)   |         |
| Київська область          |    101    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-kyivska.geojson)   |         |
| Кіровоградська область    |    145    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-kirovogradska.geojson)  |         |
| Луганська область         |    114    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-luganska.geojson)   |         |
| Львівська область         |    310    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-lvivska.geojson)   |         |
| Миколаївська область      |    786    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-mykolayivska.geojson)   |         |
| Одеська область           |    76     |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-odeska.geojson)   |         |
| Полтавська область        |    252    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-poltavska.geojson)   |         |
| Рівненська область        |    233    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-rivnenska.geojson)   |         |
| Сумська область           |    136    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-sumska.geojson)   |         |
| Тернопільська область     |    498    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-ternopilska.geojson)   |         |
| Харківська область        |    178    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-kharkivska.geojson)   |         |
| Херсонська область        |    51     |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-khersonska.geojson)   |         |
| Хмельницька область       |    308    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-khmelnytska.geojson)   |         |
| Черкаська область         |    385    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-cherkaska.geojson)   |         |
| Чернівецька область       |    278    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-chernivetska.geojson)   |         |
| Чернігівська область      |    609    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/pzo-chernigivska.geojson)   |         |
| Автономна республіка Крим |    73     |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PZO/geojson/fpzo-ar-krym.geojson)  |         |
| Всі регіони               |    5468   |     |         |


## Фізико-географічні об'єкти України

Дані опрацьовані та потребують уточнення.

| Регіон                    | Кількість об'єктів | GeoJSON file | Статус |
|---------------------------|:---------:|:---:|:-------:|
| [Вінницька область](https://land.gov.ua/wp-content/uploads/2018/02/Вінницька_область.7z)        |    925    | [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-vinnytska.geojson)    |         |
| [Волинська область](https://land.gov.ua/wp-content/uploads/2018/02/Волинська_область.7z)        |    8196   |   [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-volynska.geojson)  |         |
| [Дніпропетровська область](https://land.gov.ua/wp-content/uploads/2018/02/Дніпропетровська_область.7z)  |    1089   |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-dnipropetrovska.geojson)  |         |
| [Донецька область](https://land.gov.ua/wp-content/uploads/2018/02/Донецька_область.7z)          |    1224   |   [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-donetska.geojson)  |         |
| [Житомирська область](https://land.gov.ua/wp-content/uploads/2018/02/Житомирська_область.7z)       |    1587   |   [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-zhytomyrska.geojson)  |         |
| [Закарпатська область](https://land.gov.ua/wp-content/uploads/2018/02/Закарпатська_область.7z)      |    2136   | [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-zakarpatska.geojson)    |         |
| [Запорізька область](https://land.gov.ua/wp-content/uploads/2018/02/Запорізька_область.7z)       |    768    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-zaporizska.geojson)   |         |
| [Івано-Франківська область](https://land.gov.ua/wp-content/uploads/2018/02/Івано-Франківська_область.7z) |    4690   |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-ivano-frankivska.geojson)   |  багато помилок       |
| [Київська область](https://land.gov.ua/wp-content/uploads/2018/02/Київська_область.7z)          |    1264   |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-kyivska.geojson)   |         |
| [Кіровоградська область](https://land.gov.ua/wp-content/uploads/2018/02/Кіровоградська_область.7z)    |    2029   |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-kirovogradska.geojson)   |         |
| [Луганська область](https://land.gov.ua/wp-content/uploads/2018/02/Луганська_область.7z)         |    1907   |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-luganska.geojson)   |         |
| [Львівська область](https://land.gov.ua/wp-content/uploads/2018/08/Львівська_обл.7z)         |    2096   |   [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-lvivska.geojson)  |         |
| [Миколаївська область](https://land.gov.ua/wp-content/uploads/2018/02/Миколаївська_область.7z)      |    786    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-mykolaivska.geojson)   |         |
| [Одеська область](https://land.gov.ua/wp-content/uploads/2018/02/Одеська_область.7z)           |    1184   |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-odeska.geojson)   |         |
| [Полтавська область](https://land.gov.ua/wp-content/uploads/2018/02/Полтавська_область.7z)        |    928    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-poltavska.geojson)   |         |
| [Рівненська область](https://land.gov.ua/wp-content/uploads/2018/02/Рівненська_область.7z)        |    2187   |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-rivnenska.geojson)   |         |
| [Сумська область](https://land.gov.ua/wp-content/uploads/2018/02/Сумська_область.7z)           |    1328   |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-sumska.geojson)   |         |
| [Тернопільська область](https://land.gov.ua/wp-content/uploads/2018/02/Тернопільська_область.7z)     |    725    |   [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-ternopilska.geojson)  |         |
| [Харківська область](https://land.gov.ua/wp-content/uploads/2018/02/Харківська_область.7z)        |    1786   |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-kharkivska.geojson)   |         |
| [Херсонська область](https://land.gov.ua/wp-content/uploads/2018/08/Херсонська_обл.7z)       |    950    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-khersonska.geojson)   |         |
| [Хмельницька область](https://land.gov.ua/wp-content/uploads/2018/02/Хмельницька_область.7z)       |    314    |   [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-khmelnytska.geojson)  |         |
| [Черкаська область](https://land.gov.ua/wp-content/uploads/2018/02/Черкаська_область-1.7z)         |    683    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-cherkaska.geojson)   |   в роботі    |
| [Чернівецька область](https://land.gov.ua/wp-content/uploads/2018/02/Чернівецька_область.7z)       |    736    |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-chernivetska.geojson)   |         |
| [Чернігівська область](https://land.gov.ua/wp-content/uploads/2018/02/Чернігівська_область.7z)      |    1708   |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-chernigivska.geojson)   |         |
| [Автономна республіка Крим](https://land.gov.ua/wp-content/uploads/2018/02/Автономна-Республіка-Крим.7z) |    3286   |  [GeoJSON](https://github.com/gontsa/geonames-ua/blob/main/PGO/geojson/fiz-geo-ar-krym.geojson)   |         |
| Всі регіони               |   44514   |     |         |
