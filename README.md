# Accounting for Computers and Components 🖥️🔧

Windows Forms приложение для учёта компьютеров и комплектующих, написанное на **C#** (.NET Framework) с использованием **SQL Server** и **Windows Forms**.

##📷 Скриншоты интерфейса
![image](https://github.com/user-attachments/assets/78d09166-0ec7-4a65-8ee7-ec67de15b926) ![image](https://github.com/user-attachments/assets/db358a61-16c7-4a7a-8359-6525ada8147f) ![image](https://github.com/user-attachments/assets/658944c2-63b5-4003-950e-ba6a64f547b3)
![image](https://github.com/user-attachments/assets/c7198995-2229-4e11-9f20-362b17ed829b) ![image](https://github.com/user-attachments/assets/2dd01bf4-2562-4de1-9853-fa1a3e4d4b54)
##📷 Скриншоты схемы базы данных
![image](https://github.com/user-attachments/assets/4daf76ef-899b-434d-a178-e130c1577b04)


## 📌 Основные возможности
- Полнофункциональный графический интерфейс (Windows Forms) 
- Добавление, удаление и редактирование данных о компьютерах и комплектующих
- Расширенный поиск по характеристикам и параметрам
- Хранение данных в SQL Server 
- Генерация отчетов 
- Экспорт данных 

## 🛠️ Требования к системе
- **ОС:** Windows 10/11
- **Платформа:** .NET Framework 4.7.2+
- **СУБД:** Microsoft SQL Server 2019+
- **Доп. ПО:** SQL Server Management Studio (SSMS) 18+

## 📥 Установка и настройка

### 1. Скачивание проекта
1. Нажмите на кнопку `<> Code` вверху страницы репозитория
2. Выберите `Download ZIP`
3. Распакуйте архив в удобную папку

### 2. Восстановление базы данных
1. Откройте **Microsoft SQL Server Management Studio (SSMS)**
2. Подключитесь к вашему серверу SQL Server
3. Кликните правой кнопкой на `Databases` → `Import Data-tier Application`
4. Укажите путь к файлу `HRYBD.bacpac` (должен находиться в папке проекта)
5. Завершите процесс импорта


### 3. Настройка подключения к базе
1. Откройте проект в **Visual Studio**
2. Найдите файл `database.cs`
3. Обновите строку подключения:
```csharp
SqlConnection sqlConnection = new SqlConnection(@"Data Source=ВАШ_СЕРВЕР;Initial Catalog=HRYBD;Integrated Security=True;");

##❓ Частые проблемы и решения

    Ошибка подключения к базе: Проверьте правильность имени сервера и наличие прав доступа

    Файл .bacpac не найден: Убедитесь, что файл находится в корневой папке проекта

    Ошибка .NET Framework: Установите актуальную версию .NET Framework


