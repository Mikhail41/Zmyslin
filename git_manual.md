# Краткая инструкция GIT

* ## Первые шаги

  - ### После установки Git необходимо представиться:

  1.  **git config --global user.name «имя английскими буквами».**
  2.  **config --global user.email ваша почта@mail.com**

        Это очень важно сделать потому,что каждый коммит в Git содержит эту информацию.  
     Если этого не сделать, то вы не сможете работать в Git .

  - ### Инициализация локального репозитория

    Для создания нового репозитория используется следующая команда

    __git init__

    Эта команда выполняется один раз, для инициализации репозитория.

* ## Основные команды Git

    **git status** - эта команда позволяет получить информацию от git о его текущем состоянии.

    **git add** - эта команда добавляет файл или файлы к следующему коммиту.

    **git commit -m “message”** - эта команда создает коммит.
        
     >_добавление флага (-m) обязательно, иначе команда не сработает._

     Пример:
    ![Пример](Пример.PNG)


    **git log** - выводит на экран истории всех коммитов с их хеш-кодами.

    **git diff** - эта команда позволяет увидеть разницу между текущим файлом и закоммиченным файлом.

Продолжение следует...
======================
## Добавляем комманды.  
+ git checkout – эта комманда позволяет переходить от одного коммита к другому.
    > `обязательно нужно указать первые шесть символов хэш-адресса коммита,  
    > к которому переходим.`  

+ git checkout master - эта комманда позволяет  
  вернуться к актуальному состоянию и продолжить работу.  

+ git diff – эта комманда позволяет  
  увидеть разницу между текущим файлом и закоммиченным файлом

Комманды для работы с ветками в репозитории.  
--------------------------------------------  
* git branch - комманда для просмотра списка веток в репозитории.  
  
* git branch <название ветки> – комманда для создания новой ветки.  
 
* git checkout <название ветки> – этой коммандой переходим к другой ветке.  
  
* git  merge <название ветки> - этой коммандой выполняеться слияние изменений,  
  выполненых вдругой ветки, в текущую.  
  > Важно: использовать в сочетание с коммандой `git checkout <название ветки>`,  
  > то есть при помощи комманды `git checkout <название ветки>` перейти в ту ветку,  
  > в которую вы будете заливать изменения, обычно это ветка `master`. 
   
* git branch -d <название ветки> – эта комманда для удаления ветки.  
* 
Добовляем комманды для работы с удаленными репозиториями.  
---------------------------------------------------------  
+ git clone <url-адрес репозитория> -  Этой коммандой выполняем  
клонирование внешнего репозитория на локальный ПК.  
+ git pull - Этой комманда выполняет получение изменений и слияние с локальной версией.  
+ git push -Эта комманда отправляет локальную версию репозитория на внешний.  
  

