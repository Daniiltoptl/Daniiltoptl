# HyperBackPacks

**HyperBackPacks** — это плагин для создания резервных копий (бэкапов) всего сервера или отдельных папок Minecraft. Легко создавать, архивировать и сохранять резервные копии серверных данных с возможностью выбора расширения архивов. Идеально подходит для администраторов серверов, которые хотят обеспечить сохранность своих данных.

## Функции

- **Создание резервных копий** всего сервера или отдельных папок.
- **Архивирование в несколько форматов** (.zip, .tar, .rar и другие, в зависимости от конфигурации).
- Автоматическое создание резервных копий с меткой даты.
- Все файлы бэкапов будут сохраняться в папке плагина рядом с конфигурационным файлом.
- Простая настройка расширений архивов через конфиг.

## Установка

1. Скачайте файл плагина `HyperBackPacks.jar`.
2. Поместите его в папку `plugins` вашего серверного каталога.
3. Перезапустите сервер.
4. Плагин создаст файл конфигурации в папке `plugins/HyperBackPacks/config.yml`.

## Конфигурация

После первого запуска плагин создаст конфигурационный файл **config.yml** в папке `plugins/HyperBackPacks`.

Пример конфигурации:

```yaml
# config.yml

# Расширение файлов архивов (можно изменить на .zip, .tar, .rar и др.)
archive-extension: .zip

# Папка для бэкапов (оставить пустым, чтобы сохранить в папке плагина)
backup-folder: backups

# Команда для создания резервной копии всех данных сервера
commands:
  create_all:
    permission: backpacks.create
    description: Создание бэкапа всего сервера

# Путь к папке для архивации (например, "world" или другая папка)
backup-path: world
