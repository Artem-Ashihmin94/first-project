# Научиться учиться
![](img/main.png)

![npm bundle size](https://img.shields.io/bundlephobia/min/qwerty)

В данной проектной работе, в отличие от предыдущей, используются более сложные технологии, такие как iframe или animation.
Для стилей была применена классическая схема организации файловой структуры БЭМ-проектов.

**В проектной работе были использованы технологии:** 
* flexbox 
* animation (с помощью анимаций были анимированы 2 блока, которым задали равномерное, линейное вращение)
* iframe (на страницу добавлены видео из youtube)  
    - <https://www.youtube.com/watch?v=arj7oStGLkU>   
    - <https://www.youtube.com/watch?v=5MgBikgcWnY)>

![iframe](img/iframeVideo.png)

```CSS
 <div class="video__iframes">
                    <div class="video__iframe">
                        <iframe width="515" height="316" src="https://www.youtube.com/embed/arj7oStGLkU" 
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                        allowfullscreen></iframe>
                    </div>
                    <div class="video__iframe">
                        <iframe width="515" height="316" src="https://www.youtube.com/embed/5MgBikgcWnY" 
                        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                        allowfullscreen></iframe>
                    </div>
```


## Файловая структура
К `CSS` мы применили основные принципы организации и хранения кода методологии БЭМ:

![файловая структура БЭМ](img/CSSbam.png)

```CSS
@import url('../blocks/header/header.css');
@import url('../blocks/header/__title/header__title.css');
@import url('../blocks/header/__subtitle/header__subtitle.css');
```

* Блоку соответствует одна директория.
* Код модификаторов и элементов находится в отдельных файлах.
* Файлы модификаторов и элементов хранятся в отдельных директориях.
* Директория блока является корневой для поддиректорий его элементов и модификаторов.
* Имена директорий элементов начинаются с двойного подчеркивания (__).
* Имена директорий модификаторов начинаются с одинарного подчеркивания (_).
* Разделение кода на части и строгая организация файловой структуры проекта позволяет:
    - облегчить навигацию по проекту;
    - повторно использовать и переносить компоненты;
    - работать с уровнями переопределения и использовать сборку.




