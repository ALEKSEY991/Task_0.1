* ## Создание новой ветки и переход в неё

Создать новую ветку можно с помощью параметра branch, указав имя ветки.

`git branch new_branch_name`

Но Git не переключится на неё автоматически. Для автоматического перехода нужно добавить флаг `-b` и параметр `checkout`.

`git checkout -b new_branch_name`

### Просмотр списка веток

Можно просматривать полный список веток, используя параметр `branch`. Команда отобразит все ветки, отметит текущую звёздочкой (*) и выделит её цветом.

Также можно вывести список удалённых веток с помощью флага `-a`.

`git branch -a`

 ### Удаление ветки

Удалить ветку можно параметром `branch` с добавлением флага `-d` и указанием имени ветки. Если вы завершили работу над веткой и объединили её с основной, можно её удалить без потери истории. Однако, если выполнить команду удаления до слияния — в результате появится сообщение об ошибке. Этот защитный механизм предотвращает потерю доступа к файлам.

`git branch -d existing_branch_name`

Для принудительного удаления ветки используется флаг `-D` с заглавной буквой. В этом случае ветка будет удалена независимо от текущего статуса, без предупреждений.

`git branch -D existing_branch_name`

Вышеуказанные команды удаляют только локальную копию ветки. В удалённом репозитории она может сохраниться. Если хотите стереть удалённую ветку, выполните следующую команду:

`git push origin --delete existing_branch_name`

```
git branch
``` 
[<содержание](/radme.md)