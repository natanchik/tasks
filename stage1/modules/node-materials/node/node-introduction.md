## Начало работы

[HOME](../README.md)

### Устанавливаем Node.js

Ссылка для скачивания [https://nodejs.org/en/](https://nodejs.org/en/)

Скачиваем и устанавливаем последнюю LTS версию (Recommended For Most Users)

Проверяем что именно установили. Для этого проверяем версию Node.js.  
Открываем Git Bash: клик правой кнопкой по рабочему столу, в контекстном меню выбираем Git Bash Here. Если такого пункта нет, скачайте и установите Git [https://git-scm.com/downloads](https://git-scm.com/downloads).  
Выполняем команду `node -v`  
Если отображается версия Node.js, значит, с первым пунктом мы справились и Node.js установили.

### Возможные проблемы при установке

Иногда после установки Node.js команды в терминале, начинающиеся с `node`, вызывают ошибки наподобие `'node' is not recognized as an internal or external command, operable program or batch file`. В этом случае нужно добавить корректный путь к директории с Node.js в `PATH`. [Пример решения](https://love2dev.com/blog/node-is-not-recognized-as-an-internal-or-external-command/).

### Где писать код

В терминале писать не очень удобно. Как и в блокноте. Выбираем привычный VS Code, открываем терминал (вкладка `Терминал` на панели вверху, пункт `Создать терминал`), проверяем, что терминал работает. Для этого выполняем команду `node -v`.

### Режим REPL

Код можно писать и выполнять прямо в терминале.  
Такой режим называется REPL (от англ. `Read-Eval-Print-Loop` — цикл `чтение — вычисление — вывод`  
Чтобы в него перейти, выполните в терминале команду `node`  
Теперь код можно писать непосредственно в терминале, REPL вычислит введенное выражение и выведет результат. К примеру, если ввести `2 + 2` и нажать Enter, REPL выведет `4`.  
Также можно делать явный вывод в консоль при помощи уже знакомых нам методов. Так, вы можете написать

```js
console.log("Hello, world!");
```

REPL имеет некоторые полезные команды, получить информацию о которых можно, отправив команду `.help`  
Чтобы выйти из режима REPL, отправьте команду `.exit`(также для более грубого завершения процесса можно применить стандартное для используемого терминала сочетание клавиш наподобие `Ctrl + C`).  
Очистить терминал позволят такие команды, как `cls` (для стандартной командной строки Windows и Powershell), `clear` (для Bash).

### Как запустить файл

Режим REPL используется достаточно редко.  
Как правило, при помощи Node.js запускают код, размещенный в файлах.  
Создадим файл `test.js` и напишем в нём команду

```js
console.log("Hello, world!");
```

Откроем этот файл при помощи VS Code, в терминале выполним команду

```powershell
node test.js
```

Обратите внимание:

- расширение файла можно не указывать, т.е достаточно написать `node test`
- если возникла ошибка, убедитесь, что терминал открыт в той же директории, в которой находится файл `test.js`

## Задание

1. Выведите в консоль строку `"Hello, Node.js!"` используя режим REPL
2. Выведите в консоль строку `"Hello, Node.js!"` запустив при помощи Node.js файл с кодом

<details>
<summary>Пример решения</summary>

```js
console.log("Hello, Node.js!");
```

</details>
