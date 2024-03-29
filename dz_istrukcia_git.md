![Картинка git](Dop_Material/git.jpg)
*Перед прочтение нужно скачать программу, - нажмите [Скачать](https://git-scm.com/download/win)*

## Инструкция по работе с git

**Команды необходимые для начала работы**
* git -- version проверяет установку git
* git config --global user.name - кто будет рабоать с папкой.
* git config --global user.amail - и куда будет удалённо сохранять.

**Команды для работы с каталогом**
* git init создаст нужны файлы в каталоге
* git add .\ начнёт отслеживать изминения файлов
* git commit -m Коментируем изминения в файле
* git log проверка версий изминений файла
* git checkout команда для выбора сохранения файла
* git checkout master (вместо master пишим любую другую ветку в которой хотим работать) чтобы вернуться на основную ветку работы.
* git branch показывает на какой вы ветке работаете
* git log --oneline выводит все коментарии
* git --help показывает команды которые могут помоч
* git diff пмоможет посмотреть что сохранили или удалил
* git branch name - создаёт новую ветку
* git branch -M name Переименую ветку в которой работаете.
* git branch -d name - удаляет ветку
* git merge - объеденяет ветки
* git log --graph - показывает логи всех веток

**Команды ля работы текста**
* обрамляем полужирный текст знаком (**) Пример - **Вот так**
* обрамляем полужирный текст знаком (__) Пример - __Вот так__
* делаем текс курсивным знаком (*) Пример - *Вот так*
* делаем текс курсивным знаком (_) Пример - _Вот так_
* 1.2. делает нумерованный список
* Чтобы делать список в начале предложения ставим зна (*) или (+), в конце ничего не ставим.

**Горячие полезные клавиши**
* Ctrl+s сохраняет изминения в файле
* Кнопка Q когда в терминале светить end
* Стрелки вверх вних, быстрое переключение ранее написанного в терминале.
* Кнопка Tab дописывает название файла в терминале
* clear - команда для очистки терминала

**Доп материалы, которые помогут в работе**
* (.gitignore) - Как правильно пишеться, плюс ко всему, его надо создать в самом начале, и он поидеи должен идти первый везде, для того чтоб он действовал.
* Если хочешь переименовать папку в проекте, то закрывает студию, переименовывешь папку, открываешь студию, сохраняешь, комитеш и пушишь. Или, если все нужные изминения на github.com то удаляем папку и клонируем проект.
* Для тог чтобы перейти в другу папку, команда cd E:\Obuchenie\C#\exp - как пример. Или, на каждом новом проекте созданным в одном разделе, можно создавать новый терминал и обезательно его подписать чтобы не запутаться. 

**Загрузка локального репозитория на Github.com**
1. Должен быть создан акаунт на Github.com и выполнить вход на нём.
2. на сайте мы нажимаем рядом с ником знакочок + и выбираем new repository, пишим ему то название которое хотим, сохраняем.
3. Копируем ссылку созданного new repository.
4. и в терминале, в открытом нашем локальном проекте прописываем git remote add origin https://github.com/SEGARSS/Instrukcia_git.git (вот так это выглядет). После этого запросит авторитизацию, указываем те регистрационные данные, которы указывали при регитсрации на Github.com.
5. После этого прописываем команду git push -u origin master. (это загрузит наши данные на Github.com, также в конце команды написан master - что значит что изминения зальються именно с этой ветки)
6. Если в проекте, вы все эти команды сделали, то при повтором открытии проекта, уже ненужно выполнять 2.3.4, просто пользуемся командой git add.\ - сохранение, git commit -m - коментируем, git push - передача на Github.com.

**Как загружать репозиторий на комп из Github.com**
1. Заходим на Github.com, выбираем нужный нам уже созданный репозиторий, и открываем его cod (зелённая кнопка) это ссылка репозитория.
2. Локально, создаём папку новую там где хотим чтобы был данный репозиторий и открываем её.
3. В терминале прописываем команду git clone https://github.com/SEGARSS/Instrukcia_git.git (данная сылка там cod - зелённая кнопка в личном кабинете на Github)
4. Затем, нужно указать папку с виртуальном репозиторием - cd E:\Obuchenie\lekcii\Lekcii_Prac\Instrukcia_git.
5. Если мы работаем и изменяем файл на самом Github.com или с другова компа. Чтобы загрузить историю изминенияй, прописываем команду git pull
6. загружать изминения уже обычной командой git puch
7. Далее работаем стандартными командами для работы.

**Как скопировать чейто репозиторий**
1. на чужом репозитории, нажимаем на иконку Fork - таким образом копируем его к себе проект.
2. Далее данный проект разворачиваем всё, как в разделе (Как загружать репозиторий на комп из Github.com)
3. Все изминения нужно делать в таких случаях в новой ветке ( git branch name) и перейти на неё.
4. После этого в данном скопированном репозитории чужёва пользователя, создаём файл README.md и сохранить стандартными командами. 
5. Вносим изминения, какие хотим, и передаём из обратно командой git push --set-upstream origin name (name - название ветки в которой работаем и делали изминения). И у нас в провекте на Github.com  появляеться надмись Compare & pull request (Нажав на неё, она позволит отправить наше предложение по изминению файла)
