 * ## Слияние двух веток

Объединить две ветки можно параметром `merge` с указанием имени ветки. Команда объединит указанную ветку с основной.

`git merge existing_branch_name`

Если надо выполнить коммит слияния, выполните команду `git merge `с флагом `--no-ff`.

`git merge --no-ff existing_branch_name`

Указанная команда объединит заданную ветку с основной и произведёт коммит слияния. Это необходимо для фиксации всех слияний в вашем репозитории.
 
 ### Прекращение слияния при конфликте

Прервать слияние в случае конфликта можно параметром `merge` с флагом `--abort`. Он позволяет остановить процесс слияния и вернуть состояние, с которого этот процесс был начат.

`git merge --abort`

Также при конфликте слияния можно использовать параметр `reset`, чтобы восстановить конфликтующие файлы до стабильного состояния.
`git reset`

### Слияние удалённого репозитория с локальным

Слияние удалённого репозитория с локальным выполняется параметром `merge` с указанием имени удалённого репозитория.
`git merge origin`
```
git merge
``` 
[<содержание](/radme.md)