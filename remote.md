# Работа с удалённым репозиторием

## git remote
Для того чтобы внести вклад в какой-либо проект, вам требуется работать с удалёнными репозиториями. Удалённые репозитории это версии вашего *IT*-проекта, сохраненные в сети (локальной или интернет). При совместной работе над проектом предполагается внесение изменений в удаленный репозиторий.

**git remote add [имя_удаленного_репозитория] [адрес]** используется для добавления связанных удаленных репозиториев.

Например:
```bash=
git remote add origin https://github.com/avsudnichnikov/example
```

## git fetch
`git fetch` используется для получения изменений с удаленного репозитория. При этом приходит список изменений, но они не вносятся в код, используемый в локальном репозитории.

## git merge
`git merge` используется для слияния полученных изменений и локального репозитория.

## git pull
`git pull` является объединением двух последовательных команд `git fetch` и `git merge`.

## git push
`git push` производит отправку ваших изменений в репозиторий. Если вы и другой разработчик одновременно клонируете, затем он выполняет команду `push`, то, если после него вы попытаетесь выполнить команду `push`, ваш `push` точно будет отклонён. Для внесения ваших изменений вам требуется получить изменения с удалённого репозитория и слить их с вашим программным кодом.