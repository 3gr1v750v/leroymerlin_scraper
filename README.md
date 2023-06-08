# Скрепер вебсайта Леруа Мерлен (https://leroymerlin.ru/)

## Стек технологий
[![Python](https://img.shields.io/badge/-Python-464646?style=flat-square&logo=Python)](https://www.python.org/)
[![Selenium](https://img.shields.io/badge/-selenium-464646?style=flat-square&logo=Selenium&logoColor=blue)](https://www.selenium.dev/)
[![Beautifulsoup](https://img.shields.io/badge/-Beautifulsoup-464646?style=flat-square&logo=BeautifulSoup&logoColor=white)](https://www.crummy.com/software/BeautifulSoup/bs4/doc/)
[![Undetected_Chromedriver](https://img.shields.io/badge/-Undetected_Chromedriver-464646?style=flat-square&logo=GoogleChrome&logoColor=blue)](https://pypi.org/project/undetected-chromedriver/)

## Описание проекта

Веб скрепер для сайта Леруа Мерлен (https://leroymerlin.ru/). 
Использует Undetected_Chromedriver для обхода блокировки доступа со стороны вебсайта для скреперов.
Позволяет из исходной ссылки на категорию продуктов, получить данные всех продуктов, находящихся в результирующем листе.
Запись данных осуществляется в JSON формате.

Скрепер работает в режиме одного потока (пока).

### Пример выгружаемых данных

Пример фида в файле проекта: [leroymerlin_data.json](https://github.com/3gr1v750v/leroymerlin_scraper/blob/master/leroymerlin_data.json)

```
[{
    "domain": "Леруа Мерлен",
    "product_url": "https://leroymerlin.ru/product/lak-dlya-pola-v-banyah-i-saunah-akvateks-diy-sauna-bescvetnyy-1-l-18556226/",
    "product_title": "Лак для пола в банях и саунах Akvateks DIY Sauna бесцветный 1 л",
    "product_description": "<h2>Описание</h2><p><strong>Защитный состав для пола Akvateks</strong> надежно защищает деревянные полы от повреждений биологического характера (гниение, синева, плесень, грибок), температурных перепадов, деформаций в результате многократного намокания и высыхания. Состав предназначен для использования в помещениях бань и саун. Эффективно действует на новых и старых (очищенных) покрытиях из дерева, фанеры, ДСП, ДВП и прочих. Можно наносить на стены, потолок и другие поверхности, кроме полков.</p><h3>Особенности средства</h3><ul><li>Содержит в составе антисептические вещества, которые продолжают действовать даже при высоких температурах.</li><li>За счет натурального воска в составе обладает отличными водо- и грязеотталкивающими свойствами.</li><li>Снижает способность деревянных поверхностей поглощать воду.</li><li>Способствует поддержанию здорового микроклимата.</li><li>Образует паропроницаемый слой.</li><li>Не имеет запаха, безопасно, не выделяет токсины.</li></ul>",
    "price": "508",
    "page_title": "Лак для пола в банях и саунах Akvateks DIY Sauna бесцветный 1 л в Москве – купить по низкой цене в интернет-магазине Леруа Мерлен",
    "page_description": "В Леруа Мерлен Лак для пола в банях и саунах Akvateks DIY Sauna бесцветный 1 л и другие товары доступны по низким ценам. Купите в интернет-магазине в Москве по низким ценам. Подробные характеристики, калькулятор расчета, отзывы.",
    "shipping_dimensions": {
        "weight": "1.048"
    },
    "specifications": {
        "Страна производства": "Россия",
        "Объем (л)": "1",
        "Назначение": "Баня, Сауна",
        "Расход (в м² / л)": "14",
        "Цвет": "Бесцветный",
        "Состав": "Акрил",
        "Цветовая палитра": "Бесцветный / прозрачный",
        "Внешний вид": "Полуматовый",
        "Время высыхания между 2 слоями (ч)": "0.5",
        "Время полного высыхания (ч)": "72",
        "Тип упаковки": "Ведро",
        "Рекомендации по чистке": "Моющийся",
        "Тип защиты": "Создает защитный слой",
        "Тип использования": "Защита",
        "Можно использовать на": "Все типы древесины",
        "Срок годности (в месяцах)": "24",
        "Возможность колеровки онлайн": "Нет",
        "База под колеровку": "C",
        "Тип базы под колеровку": "Для ярких цветов (прозрачная)",
        "Место использования": "Внутренний",
        "Предназначен для": "Пол, Стена, Потолок"
    },
    "product_type": "Лак",
    "images": [
        "https://cdn.leroymerlin.ru/lmru/image/upload/v1668589725/lmcode/PbS093WWA0mwxI1A7OQ-vQ/18556226.png",
        "https://cdn.leroymerlin.ru/lmru/image/upload/v1514496115/lmcode/eMCa5xDpZUWjMUGgKLnCQw/18556226_01.jpg",
        "https://cdn.leroymerlin.ru/lmru/image/upload/v1668589725/lmcode/cktJQ1ynfUaOUh3mWRN94w/18556226_02.png",
        "https://cdn.leroymerlin.ru/lmru/image/upload/v1514496115/lmcode/l9XNrA2-JE6jqU_GpBV0kg/18556226_03.jpg",
        "https://cdn.leroymerlin.ru/lmru/image/upload/v1514496115/lmcode/PhTvFGbkuUmmW6FA4uiCmg/18556226_04.jpg",
        "https://cdn.leroymerlin.ru/lmru/image/upload/v1514496115/lmcode/3iPxPqdQZ0ip-4u6KvV8ZQ/18556226_05.jpg"
    ]
},]
```
### Технологии
- Python 3.10
- undetected_chromedriver 3.4.7
- Selenium 4.9.1 (версия выше 4.9.1 не поддерживается undetected_chromedriver)
- Beautiful Soup 4.12.2

### Особенности работы с сайтом

- Для работы через VPN необходимы Российские IP адреса;
- Если уменьшить задержку между обращениями до 2 секунд, сайт может заблокировать (блок пропадает при перезапуске скрепера);
- Обращение к глобальному дереву категорий можно ускорить через обращения к JSON (google: leroymerlin json);

## Установка и запуск

1. Скопируйте репозиторий и перейдите в него в командной строке:

```
git clone https://github.com/3gr1v750v/leroymerlin_scraper
```

```
cd leroymerlin_scraper
```

2. Создайте и активируйте виртуальное окружение:

```
python -m venv env
```

```
source env/bin/activate
```

3. Установите зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

4. Запустите проект:

```
python driver.py
```

5. Выгрузка данных в JSON:

Как только начнется сбор данных с страниц товаров, в консоли IDE появится счетчик текущего
состояния и общее количество продуктов. JSON фаил будет сформирован, как только закончится
сбор и пребразование контента (JSON не заполняется в процессе сбора, а формируется единым
пакетом на финальном этапе). После этого в консоль будет выведено сообщение, о том, что
JSON фаил сформирован.