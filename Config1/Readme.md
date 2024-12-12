# Работы по конфигурационному управлению
## Индивидуальное задание

Разработать эмулятор для языка оболочки ОС. Необходимо сделать работу эмулятора как можно более похожей на сеанс shell в UNIX-подобной ОС.
Эмулятор должен запускаться из реальной командной строки, а файл с виртуальной файловой системой не нужно распаковывать у пользователя.
Эмулятор принимает образ виртуальной файловой системы в виде файла формата zip. Эмулятор должен работать в режиме CLI.

### Ключами командной строки задаются:

  • Имя пользователя для показа в приглашении к вводу.
  
  • Имя компьютера для показа в приглашении к вводу.
  
  • Путь к архиву виртуальной файловой системы.
  
  • Путь к лог-файлу.
  
  • Путь к стартовому скрипту.
  
Лог-файл имеет формат csv и содержит все действия во время последнего сеанса работы с эмулятором. Для каждого действия указаны дата и время. Для каждого действия указан пользователь.

#### Необходимо поддержать в эмуляторе команды ls, cd и exit, а также следующие команды:

1. mkdir.
2. find.
3. tail.

Все функции эмулятора должны быть покрыты тестами, а для каждой из поддерживаемых команд необходимо написать 2 теста.

## Успешное выполнение тестов
![image](https://github.com/user-attachments/assets/96b011c6-efdb-4d61-86eb-d6bcbbfd85dc)

## Тестирование функций 
![image](https://github.com/user-attachments/assets/199189e8-6f07-4195-9aa1-c4b781cbd7e9)

![image](https://github.com/user-attachments/assets/92923867-9049-478c-b00a-32931b580bfd)

![image](https://github.com/user-attachments/assets/59ea2ed8-4910-44cf-9c47-33ccec5f14ec)

![image](https://github.com/user-attachments/assets/e92d0d6a-3785-428c-ab5c-247f8aad7805)

![image](https://github.com/user-attachments/assets/d077061a-e614-4dc3-864c-bd002a439ab0)

![image](https://github.com/user-attachments/assets/653feb66-336e-486e-a4d4-b02fc6a5d8e4)

![image](https://github.com/user-attachments/assets/95f0c57d-c54a-420a-9891-6e3116ca881f)

![image](https://github.com/user-attachments/assets/153954da-812c-4b73-8c24-3d119458afe4)

![image](https://github.com/user-attachments/assets/38d18fc1-712a-4b96-9bca-0994058841c2)

## Функция ls
### Действия:

1. Выводит список файлов и директорий в текущей директории.
2. Если указан аргумент -l, добавляет права доступа и размеры файлов.

## Функция cd
### Действия:

1. Обрабатывает переходы на уровень выше и переходы в корень. 

## Функция exit
### Действия:

1. Завершает выполнение программы.

## Функция mkdir
### Действия:

1. Проверяет, существует ли директория с таким именем.
2. Если директория не существует, создает ее в ZIP-архиве.

## Функция tail
### Действия:

1. Читает содержимое файла и выводит указанные строки с конца.


## Функция find
### Действия:

1. Ищет совпадения в именах файлов и папок внутри ZIP-архива.

## Доп задание
### Покрасить директории в бирюзовый, txt файлы в красный, а csv файлы в зеленый

![изображение](https://github.com/user-attachments/assets/3980fa55-9bab-4bfa-b5d9-732f66541749)


<div id="header" align="center">
  <img src="https://i.giphy.com/media/v1.Y2lkPTc5MGI3NjExb2h0anFyeHZyaHI1anljYWdkYjl3cG56Z3UxNGhzZDhocnZwZHZ6dyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/YITvqkRzjBb2KRklUw/giphy-downsized-large.gif" width="200"/>
</div>