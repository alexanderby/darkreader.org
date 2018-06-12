# Справка (Русский)

Этот документ расскажет вам об основных возможностях Дарк Ридера.

- [Часто задаваемые вопросы](#faq)
- [Контакты](#contacts)
- [Верхняя секция](#top-section)
- [Настройки фильтра](#filter-settings)
- [Настройки для конкретного сайта](#custom-site-settings)
- [Список сайтов](#site-list)
- [Вкладка Ещё](#more-tab)
- [Режимы генерации тем](#theme-generation-modes)
- [Нижняя секция](#bottom-section)
- [Использование Инструментов разработчика](#using-dev-tools)


<h2 id="top-section">Верхняя секция</h2>

<img src="/images/help/darkreader-top-section.png" alt="Верхняя секция" style="width: 15rem;" />

- Кнопка **Переключить** добавляет сайт в список исключений (либо достаёт оттуда).
- Переключатель **Вкл/Выкл** включает либо выключает расширение.
- Нажмите на ссылки под кнопками для установки **сочетаний клавиш**.
- Если кнопка переключения затемнена, это означает, что браузер блокирует расширения на данной странице.


<h2 id="filter-settings">Настройки фильтра</h2>

<img src="/images/help/darkreader-filter-settings.png" alt="Настройки фильтра" style="width: 15rem;" />

Настройте значения фильтра, которые соответствуют параметрам вашего экрана и освещению в комнате.


<h2 id="custom-site-settings">Настройки для определенного сайта</h2>

<img src="/images/help/darkreader-custom-site-settings.png" alt="Настройки для определенного сайта" style="width: 15rem;" />

Кнопка **Только для** применяет настройки только для текущего сайта.

Нажмите на кнопку, отредактируйте настройки, нажмите еще раз для отмены.


<h2 id="site-list">Список сайтов</h2>

<img src="/images/help/darkreader-site-list.png" alt="Список сайтов" style="width: 15rem;" />

- Используйте **Инвертировать только эти**, когда вы хотите, чтобы Dark Reader работал только на сайтах в списке. 
- **Не инвертировать** предотвратит работу расширения на сайтах в списке.
- Вызможные значения: `google.com, mail.google.com, google.*, google.com/maps` и т.п.
- Нажатие кнопки **Переключить** добавляет текущий сайт в этот список.

<h2 id="more-tab">Вкладка Ещё</h2>

<img src="/images/help/darkreader-more-tab.png" alt="Вкладка Ещё" style="width: 15rem;" />

- **Выберите шрифт** из списка (или введите полное имя шрифта в Firefox), нажмите галочку.
- Настройте **обводку текста**.
- Выберите режим **генерации тем**.


<h2 id="theme-generation-modes">Режимы генерации тем</h2>

<figure>
    <img src="/images/help/darkreader-theme-modes.png" alt="Фильтр+ vs. Статический vs. Динамический режим" />
    <figcaption>Фильтр+ vs. Статический vs. Динамический режим</figcaption>
</figure>

- **Фильтр** – Изначальный режим в Dark Reader основанный на CSS фильтрах.
Он **инвертирует всю страницу** и **реверсирует** определенные части назад.
Требователен к графическому процессору.
**Быстрый**, но имеет некоторые недостатки:
отключает технологию субпиксельного рендеринга,
инвертирует тёмные участки в светлые,
замедляет работу браузера на больших страницах,
не отрисовывает некоторые страницы в Firefox.
- **Фильтр+** – тот же, что и Фильтр, но основан на специальных SVG фильтрах
которые **лучше обрабатывают цвета** делая картинки менее тусклыми.
Плохо работает в Firefox.
- **Статический** – мгновенно генерирует простую тему.
- **Dynamic** – анализирует стили текущей веб-страницы, фоновые картинки, векторную графику.
Требует больше ресурсов при начальной загрузке страницы,
но выдаёт **наилучшие** визуальные результаты.
Работа над этим режимом в процессе,
но он уже отлично работает на большинстве современных сайтов.


<h2 id="bottom-section">Нижняя секция</h2>

<img src="/images/help/darkreader-footer.png" alt="Нижняя секция" style="width: 15rem;" />

- Прочтите нашу **политику конфиденциальности**, подписавайтесь на наш **Twitter**.
- **Поддержка** – Если вам нравится Dark Reader, поддержите его активную разработку.
Сбор средств ведёт Open Collective, который в настоящее время использует Stripe для осуществления платежей.
- **Новости** – оповещает об обновлениях приложения и важных событиях.
- **Инструменты разработчика** – открывает редактор правок в режим работы текущего генератора тем.


<h2 id="using-dev-tools">Использование Инструментов разработчика</h2>

Если вы знакомы с CSS селекторами, вы можете предложить правку для какого-либо веб-сайта.
Больше информации об инструментах разработчика [здесь](https://github.com/darkreader/darkreader#how-to-contribute).


<h2 id="faq">Часто задаваемые вопросы</h2>

#### Расширение просит права на чтение посещаемых сайтов

Расширению нужны данные права для возможности анализа и изменения внешнего вида веб-страниц, определения,
отключен ли текущий веб-сайт настройками пользователя или использования специальных настроек для текущего сайта.
Мы не встраиваем рекламу, не собираем данные пользователей и никуда их не отсылаем.
Исходный код расширения полностью открыт и не имеет зашифрованных мест.
Наша монетизация прозрачна и основывается на добровольной помощи от пользователей.

#### Страница магазина расширений и страницы настроек браузера остаются белыми

У расширения нет прав доступа к этим страницам.

#### Новая вкладка и тема браузера остаются светлыми

Расширение не имеет доступа к новой вкладке и теме браузера (может менять тему браузера начиная с Firefox 60).
Установите тёмную тему либо расширение, заменяющее новую вкладку, в магазине расширений.

#### Расширение вообще не работает

Если у вас установлены подобные расширения с тёмным режимом, отключите их, перезагрузите вкладки.
Нажмите значок Dark Reader, убедитесь что кнопка в правом верхнем углу установлена в положении **Вкл**.
Откройте вкладку **Список сайтов**, проверьте, что выбрано **Не инвертировать**.
Если ничего не помогает, значит всё совсем плохо, напишите нам на e-mail.

#### Сайт отображается некорректно или работает медленно

Пожалуйста, пришлите адрес сайта, скриншот, версии операционной системы и браузера на наш e-mail.
Мы постараемся определить причину, по крайней мере для популярного веб-сайта.
Также попробуйте изменить **режим генерации тем** или попробуйте использовать **Светлый режим**.
Проверьте, что сайт отсутствует в **Списке сайтов**.

#### Расширение не работает в режиме инкогнито

Откройте страницу **chrome://extensions**, найдите **Dark Reader**, нажмите **Разрешить использование в режиме инкогнито**.

#### Расширение не работает для локальных файлов

Откройте страницу **chrome://extensions**, найдите **Dark Reader**, нажмите **Разрешить открывать локальные файлы по ссылкам**.

#### Сайт совсем не отображается в режиме Фильтр

Если вы пользователь Chrome на Mac OS, обновите Mac OS до версии 10.13, это должно обновить видео драйверы.
Если вы пользователь Firefox, вероятно это баг браузера, используйте другой режим для таких сайтов.


<h2 id="contacts">Контакты</h2>

По всем вопросам пишите на [darkreaderapp@gmail.com](mailto:darkreaderapp@gmail.com)