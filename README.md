# Очистка Истории в Git

### Создайте временную ветку и перейдите в нее:

```
$ git checkout --orphan temp_branch
```

### Добавьте все файлы в новую ветку и сделайте коммит изменений:

```
$ git add -A
$ git commit -am "The first commit"
```

### Удалите `master` -ветку:

```
$ git branch -D master
```

### Переименуйте временную ветку в `master`:

```
$ git branch -m master
```

### Принудительно обновите удаленный репозиторий:

```
$ git push -f origin master
```
