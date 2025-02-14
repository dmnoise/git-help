
![](https://i.ibb.co/M6M3Y3q/free-png-ru-19.png)

> [!NOTE]
> Для начала нам понадобится программа Терминал.<br/>
> Вы можете найти его в списке приложений `Finder > Программы > Утилиты > Терминал` или же нажать `Cmd+Space`, затем ввести `terminal`.


# Список базовых команд 🗒️
| Команда | Описание |
| --- | --- |
| `pwd` | Показать текущую рабочую директорию (папку, из которой выполняется команда). |
| `ls` | Отобразить файлы и папки в текущей директории. |
| `l -a` | Отобразить файлы и папки в текущей директории, в том числе скрытые. |
| `cd first-project` | Перейти в папку `first-project` |
| `cd first-project/test` | Перейти в папку `test` внутри папки `first-project` |
| `cd ..` | Перейти на уревень выше (в родительскую папку) |
| `cd ~` | Перейти в домашнюю папку (например `/Users/Practicum`) |
| `mkdir second-project` | Создать папку `second-project` |
| `rm hello.txt` | Удалить файл `hello.txt` |
| `rmdir images` | Удалить папку `images` |
| `rm -r second-project` | Удалить папку `second-project` и все ее содержимое |
| `touch hello.txt hello2.txt hello3.txt` | Создать несколько файлов (`hello.txt`, `hello2.txt`, `hello3.txt`) |
| `echo <text>` | Вывести текст на экран, например, `echo "Hello, Practicum!"` |
| `echo <text> >> <file>` | Вывести текст в файл, например, `echo "Hello, Practicum!" >> output.txt` |
| `cat practicum.txt` | Вывести содержимое файла `practicum.txt` на экран. |
| `cp helloPracticum.txt practicum.txt` | В этом примере информация из источника `helloPracticum.txt` скопируется в назначение `practicum.txt` | 
| `mv <источник> <назначение>` | Переместить/переименовать файлы и папки |
| `tail <file>` | Показать последние строки файла |
| `history` | Показать историю введенных команд |
| `head <file>` | Показать первые строки файла |
| `man <command>` | Показать руководство по команде |
| `clear` | Очистить экран терминала |
| `rm -rf ~/Library/Developer/Xcode/DerivedData` | Удалить папку DerivedData<br/>Папка DerivedData обычно содержит временные файлы, созданные Xcode в процессе сборки и запуска проектов: скомпилированные бинарные файлы, индексы для ускорения поиска и кэшированные данные. Удаление этой папки может быть полезным, чтобы освободить место на диске или решить некоторые проблем, связанные с Xcode. При следующем запуске Xcode воссоздаст необходимые файлы в этой папке. |
<br style="padding-top:70px"/>

# Полезные лайфхаки 😎
### Tab для автодополнения
Чтобы не вводить названия файлов и папок полностью, можно начать
писать их имя и нажать клавишу `Tab`. Командная строка допишет путь
сама, если соответствующий файл или папка есть в текущей директории.
>
Например, находясь в папке
`dev`, начните вводить `cd first` и нажмите `Tab` . Если папка `first-project` есть внутри `dev`, то командная строка автоматически подставит её имя. Останется только нажать `Enter`.

### История команд
Клавиша `↑` (стрелка вверх) позволяет просматривать историю ваших
команд. Это удобно, когда вам нужно повторить или немного изменить
предыдущую команду. Можно пользоваться стрелками `↑` `↓` для поиска
команды, а затем ещё раз её выполнить.

### Перенаправление вывода в файл
Вспомогательные команды вроде `>` и `>>` позволяют перенаправлять
вывод команд в файлы. Например, `ls > files.txt` сохранит список файлов в
файл `files.txt`.

### Отмена текущего вывода
Если вы начали вводить команду и хотите ее отменить, нажмите `Control +
C`. Это вернёт вас к чистому приглашению командной строки.

### Повторение последней команды
Чтобы повторить последнюю введенную команду, можно ввести `!!`

### Навигация курсором
Чтобы быстро исправить введенное в начале строки, можно использовать
`Control + A` — команда переместит курсор в начало строки. Обратная
команда `Control + E` — переместит курсор в конец. Это поможет при
редактировании команд.
