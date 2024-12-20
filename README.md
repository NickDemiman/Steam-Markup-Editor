# Steam Markup Editor (Редактор разметки Steam)  
Легковесный редактор разметки steam с визуализацией. Редактор поддерживает комбинации клавиш и много чего другого.  
На данный момент реализованы теги:  
- Хедеры (Ctrl + 1,2,3)  
- Жирный текст (Ctrl + B)  
- Подчеркнутый (Ctrl + U)  
- Курсив (Ctrl + I)  
- Зачеркнутый (Ctrl + S)  
- Спойлер  
- Сырой текст (Noparse)  
- Горизонтальный разделитель  
- Формат кода  

Проектом давно не занимался и работы еще много. В плане, реализовать:  
- Url, вставка ссылок
- Маркированный списки
- Нумерованные списки
- Цитаты
- Таблицы  

Также в процессе буду фиксить ошибки и баги, которые встречу

# Быстрый старт
Проект можно опробовать следующим образом

Клонируем репозиторий  
```bash
mkdir steam-markup-editor
cd steam-markup-editor
git clone https://github.com/NickDemiman/Steam-Markup-Editor.git .
```

## Сервер Next.js
Устанавливаем зависимости
```bash
npm ci
```

Запускаем билд и сервим приложение
```bash
npm run build
npm start
```

## Docker образ
Для запуска, достаточно собрать и запустить  
```bash
docker build -t editor .
docker run -it --rm -p 8000:8000 editor:latest
```  

Либо запулить образ и запустить
```bash
docker pull ghcr.io/nickdemiman/steam-markup-editor
docker run -it --rm -p 8000:8000 ghcr.io/nickdemiman/steam-markup-editor
```
