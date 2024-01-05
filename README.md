Учебный проект ToDOList. Реализованы следующее - Веб-сервис предоставляет следующие API-эндпоинты:
    - Создание новой задачи
    - Получение списка всех задач
    - Получение задачи по идентификатору
    - Обновление задачи
    - Удаление задачи
- В каждой задаче представлены следующие атрибуты:
    - Идентификатор задачи
    - Название задачи
    - Описание задачи
    - Дата создания задачи
Добавлены возможность прикрепления файлов к задачам. Реализована сортировка и фильтрация задач по различным атрибутам. Добавлена возможность добавления к задачам категорий или меток.
1. Загрузка и конвертация PDF файлов:
- Добавлена в API возможность загружать PDF файлы в новую задачу или добавлять к уже созданным задачам.
- После загрузки PDF файлов произведится их конвертацию в изображения, обеспечивая разделение на отдельные страницы, если PDF содержит несколько страниц.
2. Интеграция с обработкой файлов:
- После конвертации PDF в изображения, изображения сохраняются в хранилище данных вместе с информацией о соответствии задаче и изображениям.
- Реализован механизм для связывания созданных изображений с соответствующей задачей.
3. Экспорт и импорт задач:
- Созданы API-методы для экспорта задачи в виде ZIP-архива, содержащего JSON файл с информацией о задаче и конвертированные изображения.
- Экспортированный ZIP-архив содержит все необходимые файлы и структуру для воссоздания задачи, включая метаданные задачи и изображения в формате, который легко можно импортировать обратно в систему(реализована создание кастомного json).
Кроме того, реализованда возможность импортирование задачи из предоставленного ZIP-архива.