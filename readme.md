# Инструкция

Расположение кода -- https://github.com/Palit-Invalid/sf_gitconfig

Склонировать репозиторий:
```bash
git clone git@github.com:Palit-Invalid/sf_gitconfig.git
```

Предварительно импортируйте свой открытый SSH-ключ в свою учётную запись на [GitHub](https://github.com)

# Процесс внесения изменений
Внесение изменений в главную ветку `master` запрещено!
Правильный алогиритм действий будет такой:

1. Создать свою ветку по шаблону: <номер_задачи>_<описание_из_двух_четырёх_слов>. Например, `DO-0001-add-debug-logging`.
2. Внести необходимые изменения и запушить их в основной репозиторий.
3. Создать Merge Request и дождаться аппрува хотя бы от одного человека.
4. Слить изменения в основную ветку `master`.

# Загрузка конфигурации Git
Конфиг [расположен](https://github.com/Palit-Invalid/sf_gitconfig/blob/master/.gitconfig) в корне репозитория
```bash
git config --local include.path "/path/to/config"
```


# Памятка по работу с Git для новичков

## Создание ветки
```bash
git checkout -b <new-branch>
```

## Внесение изменений
```bash
git add <changed-or-new_file.txt> && \
git commit -m "Some message"
```

## Слияние веток
```bash
git checkout <target-branch> # Ветка, в которую будут вливаться изменения
git merge <base-branch> # Ветка, из которой будут вливаться изменения
```