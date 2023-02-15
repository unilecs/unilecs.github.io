Тема: [Mediumish](https://github.com/wowthemesnet/mediumish-theme-jekyll/)

## Плагины
Плагинов кроме как jekyll-gist тут не использовано, его настраивать не надо. 
На счёт пагинации - [jekyll-paginate-v2](https://github.com/sverrirs/jekyll-paginate-v2) это тот плагин с 500 звёздами в гитхаб. 

Его нужно установить с помощью rubygems:
```shell
gem install jekyll-paginate-v2
```
И добавить `plugins:` в `_config.yml`.

-----
## Посты
Все посты нужно класть в папку _posts в виде `.md` файлов с названием в формате `yyyy-mm-dd-url-to-page.md`.
Сверху каждого файла настройки:
```markdown
---
layout: post
title:  "Головоломка: Пять Чисел"
categories: [ puzzles ]
tags: [numbers]
type: puzzle
featured: true
image: assets/images/five-numbers.png
---
```
Где

- **layout** - это всегда post, но можно добавить новый лэйаут в папку `_layouts` и изменить хедер с футером для отдельного поста
- **title** - название; Оно и в карде поста и сверху во вкладке 
- **categories** - разделение на категории для пагинации (пока не надо)
- **tags** - тоже пока не надо, но потом можно будет сделать страницу с постами с отдельными тегами
- **type** - task/puzzle.
- **featured** - true если пост должен отображаться на главной странице

Дальше идёт само содержание поста в виде обычного маркдауна.

-------

## Гисты

Для добавления гиста вставляем
```markdown
{% gist gist-hash-goes-brrrr %}
```
в то место где должен показываться гист. 