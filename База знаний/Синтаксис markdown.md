---
order: 200
icon: file
---

# Markdown

## Markdown - это легкий язык разметки, который используется для форматирования текста. 

Он был создан Джоном Грубером и Аароном Шварцем в 2004 году с целью создания простого и понятного способа написания веб-текстов с использованием простых символов. Markdown используется во многих платформах, включая GitHub, Reddit, Stack Overflow и многие другие.

Одна из особенностей синтаксиса Markdown заключается в том, что он не требует использования специального программного обеспечения для просмотра, поскольку любой текстовый редактор может отображать Markdown-документы в качестве форматированного текста.

Основные элементы форматирования в языке Markdown включают в себя:

### Заголовки

Заголовки обозначаются с помощью символа `#`. В Markdown есть шесть уровней заголовков, которые обозначаются **от одной до шести** символов `#`. Например:

```markdown
# Заголовок первого уровня
## Заголовок второго уровня
### Заголовок третьего уровня
```

### Абзацы

Абзацы в Markdown создаются просто путем разделения текста пустой строкой.

> По при создании абзаца, Markdown автоматически делает отступ. Чтобы начать писать с новой строки, но без отступа, используется **два пробела**.

### Списки

Markdown поддерживает упорядоченные и неупорядоченные списки. Для создания неупорядоченного списка используйте символы `*`, `-` или `+`. Для упорядоченного списка используйте числа с точкой или закрывающие скобки. Например:

```markdown
- Первый элемент списка
- Второй элемент списка
- Третий элемент списка

1. Первый элемент упорядоченного списка
2. Второй элемент упорядоченного списка
3. Третий элемент упорядоченного списка
```

Для того, чтобы создавать иерархический список необходимо использовать  "Tab"

```markdown
* Первый элемент списка
   * Подчиненный элемент списка
        * Подчиненный элемент списка
```

Выглядит это так:

* Первый элемент списка
   * Второй элемент списка
        * Третий элемент списка

### Ссылки

Ссылки в Markdown создаются, заключая текст ссылки в квадратные скобки, а URL ссылки в круглые скобки.(Пример 1) Например:

```markdown
[Текст ссылки](https://softonit.ru/)
[Сайт Softonit](https://softonit.ru/ "Сайт Softonit")
https://softonit.ru
```

Так же, можно добавить всплывающую подсказку для ссылки. Для этого, просто после URL, просто добавьте текст подсказки в кавычках.   

### Изображения

Изображения в Markdown создаются, используя символ `!`, квадратные скобки для альтернативного текста изображения и круглые скобки для URL-адреса изображения. Например:

```markdown
![Альтернативный текст](https://example.com/image.jpg)
```

### Жирный и курсивный текст

Жирный текст обозначается двумя звездочками или двумя подчеркиваниями вокруг текста, а курсивный текст обозначается одной звездочкой или одним подчеркиванием. И есть жирный курсив,который обозначается тремя звездочками или подчеркиваниями.
 Например:

```markdown
**Жирный текст**
_Курсивный текст_
***Жирный курсив***
```

### Выделение текста

- Для создания зачеркнутой строки в языке Markdown можно использовать две тильды (~~) перед и после текста.
- Для создания выделенной желтым строки в языке Markdown можно использовать несколько подряд идущих знаков равно, два или более (==) перед и после текста.
- Для создания подчеркнутого текста в языке Markdown используется два подряд идущих знаков крышечки (^), перед и после текста.

Например:

```markdown
- ~~Зачеркнутая строка~~
- ==Выделенный текст==
- ^^Подчеркнутый текст^^

```

- ~~Зачеркнутая строка~~
- ==Выделенный текст==
- ^^Подчеркнутый текст^^

### Подстрочные и надстрочные символы

Когда включены символы каретки и тильды, текст может быть дополнен вложенными и надстрочными знаками с помощью простого синтаксиса, что более удобно, чем прямое использование соответствующих HTML-тегов sub и sup:

Текст с вложенными и надстрочными знаками:

```markdown
- H~2~O
- A^T^A
```

- H~2~O
- A^T^A

### Цитаты

Цитаты в Markdown создаются с помощью символа `>`. Например:

```markdown
> Это цитата.
```

### Блок кода

Для обозначения блока кода в Markdown, код заключается в три обратных кавычки (` ``` `). 
Для оформления языка, после первых кавычек пишется расширения языка (Для 1с используется bsl)
Например:

```bsl
&НаКлиенте
Процедура СообщениеПользователю() Экспорт
 
    Сообщить("Привет, я процедура");
 
КонецПроцедуры
```

### Чекбоксы

В языке Markdown можно создавать чекбоксы для списков задач или планов. Для создания чекбокса используется тире или звездочка + символ [ ] или [x], где [ ] представляет невыполненную задачу, а [x] - выполненную задачу. Вот пример:

- [ ] Задача 1
- [x] Задача 2
- [ ] Задача 3

Результат будет выглядеть следующим образом:

```markdown
- [ ] Задача 1
- [x] Задача 2
- [ ] Задача 3
```

### Таблицы

Для создания таблицы используются вертикальные черты (|) для разделения столбцов и дефисы (-) для разделения заголовка таблицы от содержимого.

Пример таблицы в Markdown:

```
| Заголовок 1 | Заголовок 2  | Заголовок 3 |
|-------------|--------------|-------------|
| Содержимое 1| Содержимое 2 | Содержимое 3|
| Содержимое 4| Содержимое 5 | Содержимое 6|
```

Результат будет выглядеть следующим образом:

| Заголовок 1 | Заголовок 2  | Заголовок 3 |
|-------------|--------------|-------------|
| Содержимое 1| Содержимое 2 | Содержимое 3|
| Содержимое 4| Содержимое 5 | Содержимое 6|

Вы можете настроить выравнивание текста в столбцах, добавив двоеточие перед и/или после дефиса разделения заголовков и дефиса разделения содержимого. Например:

```markdown
| Заголовок 1 | Заголовок 2  | Заголовок 3 |
|:-----------:|:------------:|:-----------:|
| 1           |  2           |  3          |
| 4           |  5           |  6          |
```

### Экранирование

Markdown есть несколько символов, которые используются для форматирования текста. Если вам нужно использовать эти символы буквально, а не в качестве элементов форматирования, вы можете экранировать их с помощью обратного слэша `\`.

Вот список символов, которые могут требовать экранирования:

`\*_{}[]<>()#+-.! |`

### Inline (инлайн) код

Инлайн код в языке Markdown используется для вставки фрагментов кода прямо в текстовую строку, без отображения его в виде отдельного блока или отступа. Использование инлайн кода полезно, когда вы хотите выделить отдельный кодовый термин, переменную, функцию или другой участок кода внутри обычного текста.

Для создания инлайн кода в Markdown используются обратные одинарные кавычки \`console.log()\`, то есть косые одинаковые символы, которые обрамляют кодовый фрагмент. Например:

Результат будет выглядеть следующим образом:

Выделенный текст `console.log()`

Вот мы и познакомились с языком Markdown. Удачи в написании статей.

### Icon (иконки)

Мы используем иконки для вставки в тексте `:icon-название-иконки:`, где название-иконки - это название значка [Octicons](https://primer.github.io/octicons/).

Примеры:

* `:icon-alert:` :icon-alert:
* `:icon-star:` :icon-star:
* `:icon-cloud:` :icon-cloud:
* ...

#### Поддерживаемые иконки

В настоящее время поддерживаются следующие значки:

| URL                                                               | Shortcode              | Sample             |
| :---------------------------------------------------------------: | ---------------------- | ------------------ |
| [URL](https://primer.github.io/octicons/alert-24)                 | alert                  | `:icon-alert:` |
| [URL](https://primer.github.io/octicons/alert-fill-24)            | alert-fill             | `:icon-alert-fill:` |
| [URL](https://primer.github.io/octicons/archive-24) | archive | `:icon-archive:` |
| [URL](https://primer.github.io/octicons/arrow-both-24) | arrow-both | `:icon-arrow-both:` |
| [URL](https://primer.github.io/octicons/arrow-down-24) | arrow-down | `:icon-arrow-down:` |
| [URL](https://primer.github.io/octicons/arrow-down-left-24) | arrow-down-left | `:icon-arrow-down-left:` |
| [URL](https://primer.github.io/octicons/arrow-down-right-24) | arrow-down-right | `:icon-arrow-down-right:` |
| [URL](https://primer.github.io/octicons/arrow-left-24) | arrow-left | `:icon-arrow-left:` |
| [URL](https://primer.github.io/octicons/arrow-right-24) | arrow-right | `:icon-arrow-right:` |
| [URL](https://primer.github.io/octicons/arrow-switch-24) | arrow-switch | `:icon-arrow-switch:` |
| [URL](https://primer.github.io/octicons/arrow-up-24) | arrow-up | `:icon-arrow-up:` |
| [URL](https://primer.github.io/octicons/arrow-up-left-24) | arrow-up-left | `:icon-arrow-up-left:` |
| [URL](https://primer.github.io/octicons/arrow-up-right-24) | arrow-up-right | `:icon-arrow-up-right:` |
| [URL](https://primer.github.io/octicons/beaker-24) | beaker | `:icon-beaker:` |
| [URL](https://primer.github.io/octicons/bell-24) | bell | `:icon-bell:` |
| [URL](https://primer.github.io/octicons/bell-fill-24) | bell-fill | `:icon-bell-fill:` |
| [URL](https://primer.github.io/octicons/bell-slash-24) | bell-slash | `:icon-bell-slash:` |
| [URL](https://primer.github.io/octicons/blocked-24) | blocked | `:icon-blocked:` |
| [URL](https://primer.github.io/octicons/bold-24) | bold | `:icon-bold:` |
| [URL](https://primer.github.io/octicons/book-24) | book | `:icon-book:` |
| [URL](https://primer.github.io/octicons/bookmark-24) | bookmark | `:icon-bookmark:` |
| [URL](https://primer.github.io/octicons/bookmark-fill-24) | bookmark-fill | `:icon-bookmark-fill:` |
| [URL](https://primer.github.io/octicons/bookmark-slash-24) | bookmark-slash | `:icon-bookmark-slash:` |
| [URL](https://primer.github.io/octicons/bookmark-slash-fill-24) | bookmark-slash-fill | `:icon-bookmark-slash-fill:` |
| [URL](https://primer.github.io/octicons/briefcase-24) | briefcase | `:icon-briefcase:` |
| [URL](https://primer.github.io/octicons/broadcast-24) | broadcast | `:icon-broadcast:` |
| [URL](https://primer.github.io/octicons/browser-24) | browser | `:icon-browser:` |
| [URL](https://primer.github.io/octicons/bug-24) | bug | `:icon-bug:` |
| [URL](https://primer.github.io/octicons/calendar-24) | calendar | `:icon-calendar:` |
| [URL](https://primer.github.io/octicons/check-24) | check | `:icon-check:` |
| [URL](https://primer.github.io/octicons/check-circle-24) | check-circle | `:icon-check-circle:` |
| [URL](https://primer.github.io/octicons/check-circle-fill-24) | check-circle-fill | `:icon-check-circle-fill:` |
| [URL](https://primer.github.io/octicons/checkbox-24) | checkbox | `:icon-checkbox:` |
| [URL](https://primer.github.io/octicons/checklist-24) | checklist | `:icon-checklist:` |
| [URL](https://primer.github.io/octicons/chevron-down-24) | chevron-down | `:icon-chevron-down:` |
| [URL](https://primer.github.io/octicons/chevron-left-24) | chevron-left | `:icon-chevron-left:` |
| [URL](https://primer.github.io/octicons/chevron-right-24) | chevron-right | `:icon-chevron-right:` |
| [URL](https://primer.github.io/octicons/chevron-up-24) | chevron-up | `:icon-chevron-up:` |
| [URL](https://primer.github.io/octicons/circle-24) | circle | `:icon-circle:` |
| [URL](https://primer.github.io/octicons/circle-slash-24) | circle-slash | `:icon-circle-slash:` |
| [URL](https://primer.github.io/octicons/clock-24) | clock | `:icon-clock:` |
| [URL](https://primer.github.io/octicons/clock-fill-24) | clock-fill | `:icon-clock-fill:` |
| [URL](https://primer.github.io/octicons/cloud-24) | cloud | `:icon-cloud:` |
| [URL](https://primer.github.io/octicons/cloud-offline-24) | cloud-offline | `:icon-cloud-offline:` |
| [URL](https://primer.github.io/octicons/code-24) | code | `:icon-code:` |
| [URL](https://primer.github.io/octicons/code-of-conduct-24) | code-of-conduct | `:icon-code-of-conduct:` |
| [URL](https://primer.github.io/octicons/code-review-24) | code-review | `:icon-code-review:` |
| [URL](https://primer.github.io/octicons/code-square-24) | code-square | `:icon-code-square:` |
| [URL](https://primer.github.io/octicons/codescan-24) | codescan | `:icon-codescan:` |
| [URL](https://primer.github.io/octicons/codescan-checkmark-24) | codescan-checkmark | `:icon-codescan-checkmark:` |
| [URL](https://primer.github.io/octicons/codespaces-24) | codespaces | `:icon-codespaces:` |
| [URL](https://primer.github.io/octicons/columns-24) | columns | `:icon-columns:` |
| [URL](https://primer.github.io/octicons/command-palette-24) | command-palette | `:icon-command-palette:` |
| [URL](https://primer.github.io/octicons/comment-24) | comment | `:icon-comment:` |
| [URL](https://primer.github.io/octicons/comment-discussion-24) | comment-discussion | `:icon-comment-discussion:` |
| [URL](https://primer.github.io/octicons/commit-24) | commit | `:icon-commit:` |
| [URL](https://primer.github.io/octicons/container-24) | container | `:icon-container:` |
| [URL](https://primer.github.io/octicons/copilot-24) | copilot | `:icon-copilot:` |
| [URL](https://primer.github.io/octicons/copy-24) | copy | `:icon-copy:` |
| [URL](https://primer.github.io/octicons/cpu-24) | cpu | `:icon-cpu:` |
| [URL](https://primer.github.io/octicons/credit-card-24) | credit-card | `:icon-credit-card:` |
| [URL](https://primer.github.io/octicons/cross-reference-24) | cross-reference | `:icon-cross-reference:` |
| [URL](https://primer.github.io/octicons/dash-24) | dash | `:icon-dash:` |
| [URL](https://primer.github.io/octicons/database-24) | database | `:icon-database:` |
| [URL](https://primer.github.io/octicons/dependabot-24) | dependabot | `:icon-dependabot:` |
| [URL](https://primer.github.io/octicons/desktop-download-24) | desktop-download | `:icon-desktop-download:` |
| [URL](https://primer.github.io/octicons/device-camera-video-24) | device-camera-video | `:icon-device-camera-video:` |
| [URL](https://primer.github.io/octicons/device-desktop-24) | device-desktop | `:icon-device-desktop:` |
| [URL](https://primer.github.io/octicons/device-mobile-24) | device-mobile | `:icon-device-mobile:` |
| [URL](https://primer.github.io/octicons/devices-24) | devices | `:icon-devices:` |
| [URL](https://primer.github.io/octicons/diamond-24) | diamond | `:icon-diamond:` |
| [URL](https://primer.github.io/octicons/diff-24) | diff | `:icon-diff:` |
| [URL](https://primer.github.io/octicons/discussion-closed-24) | discussion-closed | `:icon-discussion-closed:` |
| [URL](https://primer.github.io/octicons/discussion-duplicate-24) | discussion-duplicate | `:icon-discussion-duplicate:` |
| [URL](https://primer.github.io/octicons/discussion-outdated-24) | discussion-outdated | `:icon-discussion-outdated:` |
| [URL](https://primer.github.io/octicons/dot-24) | dot | `:icon-dot:` |
| [URL](https://primer.github.io/octicons/dot-fill-24) | dot-fill | `:icon-dot-fill:` |
| [URL](https://primer.github.io/octicons/download-24) | download | `:icon-download:` |
| [URL](https://primer.github.io/octicons/duplicate-24) | duplicate | `:icon-duplicate:` |
| [URL](https://primer.github.io/octicons/eye-24) | eye | `:icon-eye:` |
| [URL](https://primer.github.io/octicons/eye-closed-24) | eye-closed | `:icon-eye-closed:` |
| [URL](https://primer.github.io/octicons/file-24) | file | `:icon-file:` |
| [URL](https://primer.github.io/octicons/file-binary-24) | file-binary | `:icon-file-binary:` |
| [URL](https://primer.github.io/octicons/file-code-24) | file-code | `:icon-file-code:` |
| [URL](https://primer.github.io/octicons/file-diff-24) | file-diff | `:icon-file-diff:` |
| [URL](https://primer.github.io/octicons/file-directory-24) | file-directory | `:icon-file-directory:` |
| [URL](https://primer.github.io/octicons/file-directory-fill-24) | file-directory-fill | `:icon-file-directory-fill:` |
| [URL](https://primer.github.io/octicons/file-directory-symlink-24) | file-directory-symlink | `:icon-file-directory-symlink:` |
| [URL](https://primer.github.io/octicons/file-media-24) | file-media | `:icon-file-media:` |
| [URL](https://primer.github.io/octicons/file-submodule-24) | file-submodule | `:icon-file-submodule:` |
| [URL](https://primer.github.io/octicons/file-symlink-file-24) | file-symlink-file | `:icon-file-symlink-file:` |
| [URL](https://primer.github.io/octicons/file-zip-24) | file-zip | `:icon-file-zip:` |
| [URL](https://primer.github.io/octicons/filter-24) | filter | `:icon-filter:` |
| [URL](https://primer.github.io/octicons/filter-remove-24) | filter-remove | `:icon-filter-remove:` |
| [URL](https://primer.github.io/octicons/flame-24) | flame | `:icon-flame:` |
| [URL](https://primer.github.io/octicons/fold-24) | fold | `:icon-fold:` |
| [URL](https://primer.github.io/octicons/fold-down-24) | fold-down | `:icon-fold-down:` |
| [URL](https://primer.github.io/octicons/fold-up-24) | fold-up | `:icon-fold-up:` |
| [URL](https://primer.github.io/octicons/gear-24) | gear | `:icon-gear:` |
| [URL](https://primer.github.io/octicons/gift-24) | gift | `:icon-gift:` |
| [URL](https://primer.github.io/octicons/git-branch-24) | git-branch | `:icon-git-branch:` |
| [URL](https://primer.github.io/octicons/git-commit-24) | git-commit | `:icon-git-commit:` |
| [URL](https://primer.github.io/octicons/git-compare-24) | git-compare | `:icon-git-compare:` |
| [URL](https://primer.github.io/octicons/git-merge-24) | git-merge | `:icon-git-merge:` |
| [URL](https://primer.github.io/octicons/git-merge-queue-24) | git-merge-queue | `:icon-git-merge-queue:` |
| [URL](https://primer.github.io/octicons/git-pull-request-24) | git-pull-request | `:icon-git-pull-request:` |
| [URL](https://primer.github.io/octicons/git-pull-request-closed-24) | git-pull-request-closed | `:icon-git-pull-request-closed:` |
| [URL](https://primer.github.io/octicons/git-pull-request-draft-24) | git-pull-request-draft | `:icon-git-pull-request-draft:` |
| [URL](https://primer.github.io/octicons/globe-24) | globe | `:icon-globe:` |
| [URL](https://primer.github.io/octicons/goal-24) | goal | `:icon-goal:` |
| [URL](https://primer.github.io/octicons/grabber-24) | grabber | `:icon-grabber:` |
| [URL](https://primer.github.io/octicons/graph-24) | graph | `:icon-graph:` |
| [URL](https://primer.github.io/octicons/hash-24) | hash | `:icon-hash:` |
| [URL](https://primer.github.io/octicons/heading-24) | heading | `:icon-heading:` |
| [URL](https://primer.github.io/octicons/heart-24) | heart | `:icon-heart:` |
| [URL](https://primer.github.io/octicons/heart-fill-24) | heart-fill | `:icon-heart-fill:` |
| [URL](https://primer.github.io/octicons/history-24) | history | `:icon-history:` |
| [URL](https://primer.github.io/octicons/home-24) | home | `:icon-home:` |
| [URL](https://primer.github.io/octicons/home-fill-24) | home-fill | `:icon-home-fill:` |
| [URL](https://primer.github.io/octicons/horizontal-rule-24) | horizontal-rule | `:icon-horizontal-rule:` |
| [URL](https://primer.github.io/octicons/hourglass-24) | hourglass | `:icon-hourglass:` |
| [URL](https://primer.github.io/octicons/hubot-24) | hubot | `:icon-hubot:` |
| [URL](https://primer.github.io/octicons/image-24) | image | `:icon-image:` |
| [URL](https://primer.github.io/octicons/inbox-24) | inbox | `:icon-inbox:` |
| [URL](https://primer.github.io/octicons/infinity-24) | infinity | `:icon-infinity:` |
| [URL](https://primer.github.io/octicons/info-24) | info | `:icon-info:` |
| [URL](https://primer.github.io/octicons/issue-closed-24) | issue-closed | `:icon-issue-closed:` |
| [URL](https://primer.github.io/octicons/issue-draft-24) | issue-draft | `:icon-issue-draft:` |
| [URL](https://primer.github.io/octicons/issue-opened-24) | issue-opened | `:icon-issue-opened:` |
| [URL](https://primer.github.io/octicons/issue-reopened-24) | issue-reopened | `:icon-issue-reopened:` |
| [URL](https://primer.github.io/octicons/issue-tracked-by-24) | issue-tracked-by | `:icon-issue-tracked-by:` |
| [URL](https://primer.github.io/octicons/issue-tracks-24) | issue-tracks | `:icon-issue-tracks:` |
| [URL](https://primer.github.io/octicons/italic-24) | italic | `:icon-italic:` |
| [URL](https://primer.github.io/octicons/iterations-24) | iterations | `:icon-iterations:` |
| [URL](https://primer.github.io/octicons/kebab-horizontal-24) | kebab-horizontal | `:icon-kebab-horizontal:` |
| [URL](https://primer.github.io/octicons/key-24) | key | `:icon-key:` |
| [URL](https://primer.github.io/octicons/law-24) | law | `:icon-law:` |
| [URL](https://primer.github.io/octicons/light-bulb-24) | light-bulb | `:icon-light-bulb:` |
| [URL](https://primer.github.io/octicons/link-24) | link | `:icon-link:` |
| [URL](https://primer.github.io/octicons/link-external-24) | link-external | `:icon-link-external:` |
| [URL](https://primer.github.io/octicons/list-ordered-24) | list-ordered | `:icon-list-ordered:` |
| [URL](https://primer.github.io/octicons/list-unordered-24) | list-unordered | `:icon-list-unordered:` |
| [URL](https://primer.github.io/octicons/location-24) | location | `:icon-location:` |
| [URL](https://primer.github.io/octicons/lock-24) | lock | `:icon-lock:` |
| [URL](https://primer.github.io/octicons/log-24) | log | `:icon-log:` |
| [URL](https://primer.github.io/octicons/mail-24) | mail | `:icon-mail:` |
| [URL](https://primer.github.io/octicons/megaphone-24) | megaphone | `:icon-megaphone:` |
| [URL](https://primer.github.io/octicons/mention-24) | mention | `:icon-mention:` |
| [URL](https://primer.github.io/octicons/milestone-24) | milestone | `:icon-milestone:` |
| [URL](https://primer.github.io/octicons/mirror-24) | mirror | `:icon-mirror:` |
| [URL](https://primer.github.io/octicons/moon-24) | moon | `:icon-moon:` |
| [URL](https://primer.github.io/octicons/mortar-board-24) | mortar-board | `:icon-mortar-board:` |
| [URL](https://primer.github.io/octicons/move-to-bottom-24) | move-to-bottom | `:icon-move-to-bottom:` |
| [URL](https://primer.github.io/octicons/move-to-end-24) | move-to-end | `:icon-move-to-end:` |
| [URL](https://primer.github.io/octicons/move-to-start-24) | move-to-start | `:icon-move-to-start:` |
| [URL](https://primer.github.io/octicons/move-to-top-24) | move-to-top | `:icon-move-to-top:` |
| [URL](https://primer.github.io/octicons/multi-select-24) | multi-select | `:icon-multi-select:` |
| [URL](https://primer.github.io/octicons/mute-24) | mute | `:icon-mute:` |
| [URL](https://primer.github.io/octicons/no-entry-24) | no-entry | `:icon-no-entry:` |
| [URL](https://primer.github.io/octicons/north-star-24) | north-star | `:icon-north-star:` |
| [URL](https://primer.github.io/octicons/note-24) | note | `:icon-note:` |
| [URL](https://primer.github.io/octicons/number-24) | number | `:icon-number:` |
| [URL](https://primer.github.io/octicons/organization-24) | organization | `:icon-organization:` |
| [URL](https://primer.github.io/octicons/package-24) | package | `:icon-package:` |
| [URL](https://primer.github.io/octicons/package-dependencies-24) | package-dependencies | `:icon-package-dependencies:` |
| [URL](https://primer.github.io/octicons/package-dependents-24) | package-dependents | `:icon-package-dependents:` |
| [URL](https://primer.github.io/octicons/paper-airplane-24) | paper-airplane | `:icon-paper-airplane:` |
| [URL](https://primer.github.io/octicons/paperclip-24) | paperclip | `:icon-paperclip:` |
| [URL](https://primer.github.io/octicons/passkey-fill-24) | passkey-fill | `:icon-passkey-fill:` |
| [URL](https://primer.github.io/octicons/paste-24) | paste | `:icon-paste:` |
| [URL](https://primer.github.io/octicons/pencil-24) | pencil | `:icon-pencil:` |
| [URL](https://primer.github.io/octicons/people-24) | people | `:icon-people:` |
| [URL](https://primer.github.io/octicons/person-24) | person | `:icon-person:` |
| [URL](https://primer.github.io/octicons/person-add-24) | person-add | `:icon-person-add:` |
| [URL](https://primer.github.io/octicons/person-fill-24) | person-fill | `:icon-person-fill:` |
| [URL](https://primer.github.io/octicons/pin-24) | pin | `:icon-pin:` |
| [URL](https://primer.github.io/octicons/pin-slash-24) | pin-slash | `:icon-pin-slash:` |
| [URL](https://primer.github.io/octicons/pivot-column-24) | pivot-column | `:icon-pivot-column:` |
| [URL](https://primer.github.io/octicons/play-24) | play | `:icon-play:` |
| [URL](https://primer.github.io/octicons/plug-24) | plug | `:icon-plug:` |
| [URL](https://primer.github.io/octicons/plus-24) | plus | `:icon-plus:` |
| [URL](https://primer.github.io/octicons/plus-circle-24) | plus-circle | `:icon-plus-circle:` |
| [URL](https://primer.github.io/octicons/project-24) | project | `:icon-project:` |
| [URL](https://primer.github.io/octicons/project-roadmap-24) | project-roadmap | `:icon-project-roadmap:` |
| [URL](https://primer.github.io/octicons/project-symlink-24) | project-symlink | `:icon-project-symlink:` |
| [URL](https://primer.github.io/octicons/project-template-24) | project-template | `:icon-project-template:` |
| [URL](https://primer.github.io/octicons/pulse-24) | pulse | `:icon-pulse:` |
| [URL](https://primer.github.io/octicons/question-24) | question | `:icon-question:` |
| [URL](https://primer.github.io/octicons/quote-24) | quote | `:icon-quote:` |
| [URL](https://primer.github.io/octicons/read-24) | read | `:icon-read:` |
| [URL](https://primer.github.io/octicons/rel-file-path-24) | rel-file-path | `:icon-rel-file-path:` |
| [URL](https://primer.github.io/octicons/reply-24) | reply | `:icon-reply:` |
| [URL](https://primer.github.io/octicons/repo-24) | repo | `:icon-repo:` |
| [URL](https://primer.github.io/octicons/repo-clone-24) | repo-clone | `:icon-repo-clone:` |
| [URL](https://primer.github.io/octicons/repo-forked-24) | repo-forked | `:icon-repo-forked:` |
| [URL](https://primer.github.io/octicons/repo-locked-24) | repo-locked | `:icon-repo-locked:` |
| [URL](https://primer.github.io/octicons/repo-pull-24) | repo-pull | `:icon-repo-pull:` |
| [URL](https://primer.github.io/octicons/repo-push-24) | repo-push | `:icon-repo-push:` |
| [URL](https://primer.github.io/octicons/repo-template-24) | repo-template | `:icon-repo-template:` |
| [URL](https://primer.github.io/octicons/report-24) | report | `:icon-report:` |
| [URL](https://primer.github.io/octicons/rocket-24) | rocket | `:icon-rocket:` |
| [URL](https://primer.github.io/octicons/rows-24) | rows | `:icon-rows:` |
| [URL](https://primer.github.io/octicons/rss-24) | rss | `:icon-rss:` |
| [URL](https://primer.github.io/octicons/ruby-24) | ruby | `:icon-ruby:` |
| [URL](https://primer.github.io/octicons/screen-full-24) | screen-full | `:icon-screen-full:` |
| [URL](https://primer.github.io/octicons/screen-normal-24) | screen-normal | `:icon-screen-normal:` |
| [URL](https://primer.github.io/octicons/search-24) | search | `:icon-search:` |
| [URL](https://primer.github.io/octicons/server-24) | server | `:icon-server:` |
| [URL](https://primer.github.io/octicons/share-24) | share | `:icon-share:` |
| [URL](https://primer.github.io/octicons/share-android-24) | share-android | `:icon-share-android:` |
| [URL](https://primer.github.io/octicons/shield-24) | shield | `:icon-shield:` |
| [URL](https://primer.github.io/octicons/shield-check-24) | shield-check | `:icon-shield-check:` |
| [URL](https://primer.github.io/octicons/shield-lock-24) | shield-lock | `:icon-shield-lock:` |
| [URL](https://primer.github.io/octicons/shield-slash-24) | shield-slash | `:icon-shield-slash:` |
| [URL](https://primer.github.io/octicons/shield-x-24) | shield-x | `:icon-shield-x:` |
| [URL](https://primer.github.io/octicons/sidebar-collapse-24) | sidebar-collapse | `:icon-sidebar-collapse:` |
| [URL](https://primer.github.io/octicons/sidebar-expand-24) | sidebar-expand | `:icon-sidebar-expand:` |
| [URL](https://primer.github.io/octicons/sign-in-24) | sign-in | `:icon-sign-in:` |
| [URL](https://primer.github.io/octicons/sign-out-24) | sign-out | `:icon-sign-out:` |
| [URL](https://primer.github.io/octicons/single-select-24) | single-select | `:icon-single-select:` |
| [URL](https://primer.github.io/octicons/skip-24) | skip | `:icon-skip:` |
| [URL](https://primer.github.io/octicons/skip-fill-24) | skip-fill | `:icon-skip-fill:` |
| [URL](https://primer.github.io/octicons/smiley-24) | smiley | `:icon-smiley:` |
| [URL](https://primer.github.io/octicons/sort-asc-24) | sort-asc | `:icon-sort-asc:` |
| [URL](https://primer.github.io/octicons/sort-desc-24) | sort-desc | `:icon-sort-desc:` |
| [URL](https://primer.github.io/octicons/sponsor-tiers-24) | sponsor-tiers | `:icon-sponsor-tiers:` |
| [URL](https://primer.github.io/octicons/square-24) | square | `:icon-square:` |
| [URL](https://primer.github.io/octicons/square-fill-24) | square-fill | `:icon-square-fill:` |
| [URL](https://primer.github.io/octicons/squirrel-24) | squirrel | `:icon-squirrel:` |
| [URL](https://primer.github.io/octicons/stack-24) | stack | `:icon-stack:` |
| [URL](https://primer.github.io/octicons/star-24) | star | `:icon-star:` |
| [URL](https://primer.github.io/octicons/star-fill-24) | star-fill | `:icon-star-fill:` |
| [URL](https://primer.github.io/octicons/stop-24) | stop | `:icon-stop:` |
| [URL](https://primer.github.io/octicons/stopwatch-24) | stopwatch | `:icon-stopwatch:` |
| [URL](https://primer.github.io/octicons/strikethrough-24) | strikethrough | `:icon-strikethrough:` |
| [URL](https://primer.github.io/octicons/sun-24) | sun | `:icon-sun:` |
| [URL](https://primer.github.io/octicons/sync-24) | sync | `:icon-sync:` |
| [URL](https://primer.github.io/octicons/tab-24) | tab | `:icon-tab:` |
| [URL](https://primer.github.io/octicons/table-24) | table | `:icon-table:` |
| [URL](https://primer.github.io/octicons/tag-24) | tag | `:icon-tag:` |
| [URL](https://primer.github.io/octicons/tasklist-24) | tasklist | `:icon-tasklist:` |
| [URL](https://primer.github.io/octicons/telescope-24) | telescope | `:icon-telescope:` |
| [URL](https://primer.github.io/octicons/telescope-fill-24) | telescope-fill | `:icon-telescope-fill:` |
| [URL](https://primer.github.io/octicons/terminal-24) | terminal | `:icon-terminal:` |
| [URL](https://primer.github.io/octicons/thumbsdown-24) | thumbsdown | `:icon-thumbsdown:` |
| [URL](https://primer.github.io/octicons/thumbsup-24) | thumbsup | `:icon-thumbsup:` |
| [URL](https://primer.github.io/octicons/tools-24) | tools | `:icon-tools:` |
| [URL](https://primer.github.io/octicons/tracked-by-closed-completed-24) | tracked-by-closed-completed | `:icon-tracked-by-closed-completed:` |
| [URL](https://primer.github.io/octicons/tracked-by-closed-not-planned-24) | tracked-by-closed-not-planned | `:icon-tracked-by-closed-not-planned:` |
| [URL](https://primer.github.io/octicons/trash-24) | trash | `:icon-trash:` |
| [URL](https://primer.github.io/octicons/triangle-down-24) | triangle-down | `:icon-triangle-down:` |
| [URL](https://primer.github.io/octicons/triangle-left-24) | triangle-left | `:icon-triangle-left:` |
| [URL](https://primer.github.io/octicons/triangle-right-24) | triangle-right | `:icon-triangle-right:` |
| [URL](https://primer.github.io/octicons/triangle-up-24) | triangle-up | `:icon-triangle-up:` |
| [URL](https://primer.github.io/octicons/trophy-24) | trophy | `:icon-trophy:` |
| [URL](https://primer.github.io/octicons/typography-24) | typography | `:icon-typography:` |
| [URL](https://primer.github.io/octicons/unfold-24) | unfold | `:icon-unfold:` |
| [URL](https://primer.github.io/octicons/unlink-24) | unlink | `:icon-unlink:` |
| [URL](https://primer.github.io/octicons/unlock-24) | unlock | `:icon-unlock:` |
| [URL](https://primer.github.io/octicons/unmute-24) | unmute | `:icon-unmute:` |
| [URL](https://primer.github.io/octicons/unread-24) | unread | `:icon-unread:` |
| [URL](https://primer.github.io/octicons/unverified-24) | unverified | `:icon-unverified:` |
| [URL](https://primer.github.io/octicons/upload-24) | upload | `:icon-upload:` |
| [URL](https://primer.github.io/octicons/verified-24) | verified | `:icon-verified:` |
| [URL](https://primer.github.io/octicons/versions-24) | versions | `:icon-versions:` |
| [URL](https://primer.github.io/octicons/video-24) | video | `:icon-video:` |
| [URL](https://primer.github.io/octicons/workflow-24) | workflow | `:icon-workflow:` |
| [URL](https://primer.github.io/octicons/x-24) | x | `:icon-x:` |
| [URL](https://primer.github.io/octicons/x-circle-24) | x-circle | `:icon-x-circle:` |
| [URL](https://primer.github.io/octicons/x-circle-fill-24) | x-circle-fill | `:icon-x-circle-fill:` |
| [URL](https://primer.github.io/octicons/zap-24) | zap | `:icon-zap:` |
| [URL](https://primer.github.io/octicons/zoom-in-24) | zoom-in | `:icon-zoom-in:` |
| [URL](https://primer.github.io/octicons/zoom-out-24) | zoom-out | `:icon-zoom-out:` |
