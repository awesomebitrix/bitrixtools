
# Утилиты для CMS Bitrix

## Установка

1) Для Windows нужно установить https://git-for-windows.github.io/

2) **Скрипт обновления утилит** - `.install` - копирует утилиты для доступа из командной строки
```
cd ~/bin
git clone https://github.com/rivetweb/bitrixtools && cd bitrixtools && ./.install
```

## Команды

Запускаются из папки модуля, например `/bitrix/modules/partner.module1`

### bitrix-php-lint

Проверка на синтаксические ошибки php-интерпретатором. Прописать в $HOME/bin/init путь к интерпретатору, например php 5.3:
```
PHPBITRIX="C:/Users/user/Bitrix/apache2/zendserver/bin/php.exe"
```

### bitrix-lang-check

Проверка на наличие кирилического текста в файлах php, папка lang не учитывается при проверке.

### bitrix-mod-new

- TODO создает пустой модуль
- id берется из названия папки
- на основе id создаются основные языковые фразы (имя модуля и пописание модуля и различные пути)

### bitrix-mod-pack

Собирает модуль в архив tar.gz, автоматически конвертирует файлы с языковыми фразами в windows-1251.

### bitrix-mod-packupdates

TODO Создает архив обновлений

### bitrix-mod-publish

TODO заливает в маркетплейс - посмотреть api или через логинится и эмулировать загрузку через форму
