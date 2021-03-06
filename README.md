ОПИСАНИЕ
--------

Плагин предназначен для рассылки приветствий новым пользователя в LiveStreet CMS.
В тексте сообщения можно благодарить пользователя за регистрацию и
дать ему ссылки на страницу помощи или общих вопросов по работе с сайтом.

Плагин совместим с плагином многоязычности l10n. Т.е. вы можете создавать разные шаблоны сообщений
для разных языков.


ЛИЦЕНЗИИ
--------

Файлы в этом архиве распостраняются по лицензии GNU GPL. Вы можете найти копию
этой лицензии в файле LICENSE.txt.


ИСТОРИЯ ВЕРСИЙ
--------------

v0.4.1
- адаптация под PHP7.2
- новая система регистрации хуков
- удалён конфиг Travis CI

v0.4.0
- адаптация под PHP7

v0.3.0
- Плагин адаптирован для работы с LiveStreet v1.0
- Добавлены тестовые сценарии и конфиг для Travis CI

v0.2.0
- Добавлена поддержка плагина l10n
- Это последняя версия, которая работает с LiveStreet v0.5.1. Скачать её можно по ссылке  https://github.com/stfalcon-studio/ls-plugin_greeting/archive/v0.2.0.zip

v0.1.0 (анонс http://livestreet.ru/blog/addons/8005.html)
- Релиз плагина

УСТАНОВКА
---------

Внесите изменения в файл настроек плагина `/plugins/greeting/config/config.php`

Для конфигурирования доступны опции:
`$config['from_user_id'] = 1;`	    // id юзера от которого будут приходить сообщения
`$config['page_name'] = 'about';`	// имя страницы ссылка на которую будет подставляться в шаблон сообщения вместо %%url%%

Настройте шаблоны сообщений, которые хранятся в директории /plugins/greeting/templates/language
В шаблонах можно использовать переменные %%name%% и %%url%%, которые будут заменены на логин пользователя
и ссылку на страницу с именем $config['page_name'].

