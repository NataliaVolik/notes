## Основные правила при верстке писем

**1. Максимальная ширина контента email-письма 600px.**

   При использовании максимальной ширины в 600 пикселей пользователям нет
   небходимости прокручивать письмо горизонтально.
   
**1. Допустимые форматы изображений .jpg, .png, .jpeg, .gif.**

   Изображение должно быть весом меньше 200Кбайт. Картинку надо сжать перед вставкой в
   письмо. Можно воспользоваться сервисом [ResizePicOnline.com](http://resizepiconline.com/) для сжатия изображений.
   По умолчанию все email-клиенты прячут изображения, поэтому в атрибуте alt=""
   можно указывать наименование изображения.
   
   
**1. Использование веб-безопасных шрифтов.**

   Веб-безопасные шрифты делятся на 4 типа или семейства: serif (с засечками),
   sans serif (без засечек), cursive (курсив), и monospace (моноширный).
   Каждый из этих типов имеют основные шрифты и резервные.
   
   Веб-безопасные шрифты с засечками (используются в основном в заголовках):

```
font-family: 'Bookman Old Style', serif;
font-family: 'Arial Black', Gadget, sans-serif;
font-family: Impact, Charcoal, sans-serif;
font-family: 'MS Sans Serif', Geneva, sans-serif;
font-family: 'MS Serif', 'New York', sans-serif;
font-family: 'Trebuchet MS', Helvetica, sans-serif;
font-family: Verdana, Geneva, sans-serif;
font-family: 'Lucida Sans Unicode', 'Lucida Grande', sans-serif;
font-family: Tahoma, Geneva, sans-serif;
```

Веб-безопасные моноширные шрифты (используются в основном для создания таблиц):
  
```
font-family: Courier, monospace;
font-family: 'Courier New', Courier, monospace;
font-family: 'Lucida Console', Monaco, monospace;
```

Веб-безопасные шрифты без засечек (используются для основного содержимого страницы):
  
```
font-family: Arial, Helvetica, sans-serif;
font-family: 'Arial Black', Gadget, sans-serif;
font-family: Impact, Charcoal, sans-serif;
font-family: 'MS Sans Serif', Geneva, sans-serif;
font-family: 'MS Serif', 'New York', sans-serif;
font-family: 'Trebuchet MS', Helvetica, sans-serif;
font-family: 'Lucida Sans Unicode', 'Lucida Grande', sans-serif;
font-family: Tahoma, Geneva, sans-serif;
```

Веб-безопасные курсивные шрифты (используют в основном чтобы выделить текст):

```
font-family: 'Comic Sans MS', cursive;
```

**4. Идеальный размер email варьируется в пределах 15 Kбайт — 100 Kбайт.**

При превышение этого лимита письмо будет попадать в спам-фильтры.

**5. Использовать простую структуру, так как есть много ограничений в html и css.**

Использовать эффекты надо осторожно поскольку не все email-клиенты понимают свойства CSS3.
Посмотреть какие свойства поддерживаются почтовыми клиентами можно в таблице по этой
[ссылке](https://www.campaignmonitor.com/css/) или например у Gmail-клиента есть справка [Gmail Supported CSS Properties and Media Queries](https://developers.google.com/gmail/design/reference/supported_css).


**6. Использование inline CSS**

Для того, чтобы HTML-версия email-рассылки корректно отображалась во всех почтовых клиентах и сервисах, необходимо привести CSS-стили HTML-кода в inline-состояние. 
Утилиты CSS Inliner например на сайте [templates.mailchimp.com](https://templates.mailchimp.com/resources/inline-css/) или [inliner.cm](https://inliner.cm/) автоматически приводит все CSS, которые есть в HTML в inline-style.

##### Email-фреймворки

[Foundation for Emails](http://foundation.zurb.com/emails.html)

[MJML](https://mjml.io/)

##### Тестирование писем

* Отсылать письмо себе на почту: 
на десктоп (Outlook), на веб-клиент (Gmail) и на мобильный клиент (iOS Mail). Можно использовать код [github.com/AlexKalinin/send-email-with-ruby](https://github.com/AlexKalinin/send-email-with-ruby) для отправки email-писем.
* Автоматически тестировать с помощью [Litmus](https://litmus.com/) или 
[Email on Acid](https://www.emailonacid.com/email-testing)
