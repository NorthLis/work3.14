[<вернуться](readme.md)
# Настройка Git


Настроить рабочую среду нужно только один раз — после обновлений параметры не сбросятся. Если понадобится, в любое время можно изменить ваши настройки.

Самый удобный способ изменения конфигурации — встроенная утилита `git config`. Настройки Git имеют три уровня:

Параметры из файла \[path]/etc/gitconfig (системные) могут работать для всех пользователей системы и репозиториев. Они редактируются командой git config —system.
Параметры из файла ~/.gitconfig или ~/.config/git/config (глобальные) применяются к одному пользователю, если запустить команду git config —global.
Локальные параметры из файла config в рабочем каталоге .git/config сохраняют только для выбранного репозитория. Ему соответствует команда `git config —local`
Если запускать `git config` без параметров, будет использоваться локальный уровень, никакие из более глобальных настроек не изменятся.

Всю используемую конфигурацию можно просмотреть так:

git config --list --show-origin

### Представимся Git, чтобы в рабочих коммитах сохранялось ваше авторство:


    git config --global user.name "Name"
    git config --global user.email @mail

[<назад](/installGit.md) [вперед>](commandGit.md)