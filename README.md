**Задание 1. Настройка блока general и sip peers**

Как практикующий dev-ops использовал вм с внешним ip адресом на Yandex Cloud

Устовка выполнялась на debian 11

По началу бфли проблемы с deprecadet chan.sip, но потмо сделал загрузку модуля chan.sip и отклбчение модуля pjsip и все завелось

Вот завел двух абонентов


[SIP.CONF](https://github.com/mezhibo/ni1004/blob/914767934acc924e1a8999ecd1b86be14e2e7c3a/IMG/sip.conf)


![Image alt](https://github.com/mezhibo/ni1004/blob/914767934acc924e1a8999ecd1b86be14e2e7c3a/IMG/1.jpg)

Абоненты готовы, но диалпалана еще нет, звонить не получится, отсюда поле с ip пустое

Сейчас создадим диалплан и посмотрим значение ip адресов абонентов

**Задание 2. Настройка плана набора**

На 2 мобильника установил Zoiper, перед этим настроив план набора

Звоню

![Image alt](https://github.com/mezhibo/ni1004/blob/914767934acc924e1a8999ecd1b86be14e2e7c3a/IMG/2.jpg)

Видно что звонок идет


Теперь глянем sip show peers и увидим что после звонков ip адреса абонентов определились


![Image alt](https://github.com/mezhibo/ni1004/blob/914767934acc924e1a8999ecd1b86be14e2e7c3a/IMG/3.jpg)
