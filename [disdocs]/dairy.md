## 23.10.2019

- Упрощена функция `dialog.sets.now`. @me{2014} #archived
- Исправлена функция `dialog.closeup`. Не отслеживалось состояние `usehtml` #archived
- Исправлена функция `dialog.replic.int`. Удалены лишние обращения к ненужным в данной версии модуля #archived
- Исключена функция `dialog.sets.now` #archived
- Упрощена функция `dialog.replic.print` #archived

+	В мануале описаны функции:
	- `dialog.int.quest`
	- `dialog.int.answer`
	- `dialog.closeup`

## 24.10.2019

+ В мануале описана функция `dialog.get.jump`
+ В мануале дополнено описания переменной `$DIALOG_VALUE['list.act.del']`

## 25.10.2019

- Переделана функция `dialog.sets.default`. Теперь она не выставляет соответствующие знчения в массив `$DIALOG_VALUE[]`. #archived
- Переделана функция `dialog.sets.attrib`. Теперь она возвращает новый набор аттрибутов на основе двух переданных. #archived
- Переработана функция/процедура `dialog.sets.transport` в соответствии с новыми механизмами. Таким образом мы избавились от множества лишних переменных, но и вместе с тем, увеличили конечный объём базы данных. #archived

+ В мануале описаны все оставшиеся функции.

## 05.04.2020

Сложная система переходов внутри хранилищ требовала хранения некоторых данных в массиве "$cvar" со сложной системой индексации, тогда как можно было использовать один простой массив для записи всех переходов по принципу системы возврата по локациям. См. вопрос "Как сделать кнопку назад" в F.A.Q.

## 11.04.2020

Можно переработать функцию сравнения массивов на выдачу разных результатов, либо разработать новую функцию, сравнивающую массивы по принципу отношения множеств. (см. отношения между понятиями в учебнике логики).

## 21.06.2020

В +lib+ easy.math подправлены локации теста и вводной. На локации теста добавлена команда извлечения корня квадратного. На вводной убраны строки со скайпом и icq. Добавить строку с адресом vk и строку со ссылкой на канал.

## 11.10.2020

В +lib+ easy.math поправлена функция get.tag.num, теперь она выдаёт более логичный результат. Так же для всех функций добавлена инициализация `$args[9]`, чтобы текстовые индексы не перезатирали числовые, особенно в новых версиях libqsp.
