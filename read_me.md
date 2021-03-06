# Gei ReadMe

## Работа с ветками

Для просмотра списков существующих веток необходимо вызвать следующую команду:

    git branch  

Команда *git status* позволяет просмотреть текущее состояние, в том числе название текущей ветки
        

### Добавление новой ветки

Для добавленич новой ветки используется следующая команда("branch_name" - название создаваемой ветки):

    git branch branch_name
    

git checkout -b branch_name - создает новую ветку и сразу переходит на нее

### Переход между ветками

Для перехода между ветками используется следующая команда ("branch_name" - название создаваемой ветки):

    git checkout branch_name

### Удаление ветки

Для удаления ветки необходимо вызвать следующую команду:("branch_name" - название удаляем ветки)

    git branch -d branch_name


   

*Внимание!* - перед удаление ветки неодходимо удостовериться, что данные созранены и данная ветка более не потребуется.

### Слияние веток

Для слияния двух веток применяется следующая команда:

    git merge branch_name

**Важные моменты при слиянии!**

* В момент слияния мы находимся в ветке, куда будут загружены изменения;
* "branch_name" - название ветки, изменения которой будут отправляться.

### Последствия слияния веток

При слиянии могут возникнуть ситуации, когда в основной ветке есть противоречия относительно изменений получаемых с побочной ветки. В таких случаях в среде VS Code нам предоставляется возможность реализовать одни из следующих вариантов:

* Оставить в основной ветке ее версию данных;

* Заменить данные основной ветки на данные влияемой ветки;
* Оставить оба варианта, для возможности вручную указать итоговые данные.
