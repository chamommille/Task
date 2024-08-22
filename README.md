
<h1 align = "center"> Git and GitHub knowledges<h1>

    
<h2 align = "center"> Basic commands <h2>
<h3>
    <table align = "center"> 
        <tr>
            <th> Command name </th>
            <th> Atributes </th>
            <th> Description </th>
        </tr>
        <tr>
            <td> pwd </td>
            <td> - </td>
            <td> Узнать путь до текущей директории </td>
        <tr>
        <tr>
            <td rowspan = "3"> cd  </td>
            <td> ~ </td>
            <td> Перейти к домашней директории </td>
        </tr>
        <tr>
            <td> .. </td>
            <td> Перейти на уровень выше </td>
        </tr>
        <tr>
            <td> / </td>
            <td> Перейти к корневой директории </td>
        </tr>
        <tr>
            <td rowspan = 2> ls </td>
            <td> -a </td>
            <td> Отобразить все файлы, в т.ч. и скрытые </td>
        </tr>
        <tr>
            <td> ~ </td>
            <td> Отобразить файлы домашней директории </td>
        </tr>
    </table>
</h3>

    
<h2 align = "center"> Create commands <h2>
<h3>
    <table align = "center"> 
        <tr>
            <th> Command name </th>
            <th> Atributes </th>
            <th> Description </th>
        </tr>
        <tr>
            <td> touch «имя файла» </td>
            <td> - </td>
            <td> Создать файл </td>
        <tr>
        <tr>
            <td rowspan = "2"> mkdir «опция» «директория / структура директорий» </td>
            <td> - </td>
            <td> Создать папку в текущей директории </td>
        </tr>
        <tr>
            <td> -р </td>
            <td> Создать структуру директорий </td>
        </tr>
    </table>
</h3>


<h2 align = "center"> Actions with files and directories hello<h2>
<h3>
    <table align = "center"> 
        <tr>
            <th> Command name </th>
            <th> Atributes </th>
            <th> Description </th>
        </tr>
        <tr>
            <td> cp «что копируем» «куда копируем» </td>
            <td> - </td>
            <td> Копирование файлов </td>
        <tr>
        <tr>
            <td> mv «что перемещаем» «куда перемещаем» </td>
            <td> - </td>
            <td> Переместить файл или папку </td>
        </tr>
        <tr>
            <td> cat «название файла» </td>
            <td> - </td>
            <td>Прочесть содержимое файла</td>
        </tr>
        <tr>
            <td rowspan = "3"> rm «файл» </td>
            <td> - </td>
            <td> Удалить файл </td>
        </tr>
        <tr>
            <td> -r </td>
            <td>Удалить папку со всем содержимым</td>
        </tr>
        <tr>
            <td> -f </td>
            <td>Удалить без вопросов</td>
        </tr>
        <tr>
            <td> rmdir </td>
            <td>-</td>
            <td>Удалить директорию при условии, что она не содержит файлы</td>
        </tr>
    </table>
</h3>

<h2 align = "center"> Git commands <h2>
<h3>
    <table align = "center"> 
        <tr>
            <th> Command name </th>
            <th> Atributes </th>
            <th> Description </th>
        </tr>
        <tr>
            <td> git init </td>
            <td> - </td>
            <td> Инициализировать репозиторий </td>
        <tr>
        <tr>
            <td> git status </td>
            <td> - </td>
            <td> Проверить состояние репозитория </td>
        </tr>
        <tr>
            <td rowspan = "3"> git add  </td>
            <td> - </td>
            <td>Подготовить файл к сохранению</td>
        </tr>
        <tr>
            <td> --all </td>
            <td> Подготовить к сохранению сразу все файлы </td>
        </tr>
        <tr>
            <td> . </td>
            <td>Добавить в репозиторий текущую папку со всеми файлами</td>
        </tr>
        <tr>
            <td> git commit </td>
            <td>-m</td>
            <td>Сохранить изменения добавленных файлов</td>
        </tr>
        <tr>
            <td> git push -u origin master </td>
            <td> - </td>
            <td>Отправить изменения на удаленный репозиторий</td>
        </tr>
    </table>
</h3>


<h2 align = "center"> SSH Key <h2>
<h3> SSH — протокол, который обеспечивает безопасный обмен данными в сети и использует для этого ключи.<h3>
<h3> SSH-ключ — ваш виртуальный идентификатор в GitHub. Как ключ от квартиры, он позволяет получить доступ к GitHub-репозиторию. Также SSH используется для доступа к другим удалённым серверам.<h3>
<h3> SSH-ключ состоит из двух частей — публичной и приватной. Публичный ключ зашифрует данные, а приватный — расшифрует. Приватным ключом ни в коем случае нельзя делиться.<h3>
<h3>
    <table align = "center"> 
        <tr>
            <th> Command name </th>
            <th> Description </th>
        </tr>
        <tr>
            <td> cd ~ </td>
            <td> Переход в домашнюю директорию </td>
        <tr>
        <tr>
            <td> ls -la .ssh </td>
            <td> Вывод список созданных ключей </td>
        </tr>
        <tr>
            <td> ssh-keygen -t ed25519 -C "Электронная почта"  </td>
            <td>Генерация SSH-пары</td>
        </tr>
        <tr>
            <td> clip < ~/.ssh/id_ed25519.pub  </td>
            <td> Скопировать публичный SSH-ключ в буфер обмена </td>
        </tr>
        <tr>
            <td> ssh -T git@github.com </td>
            <td> Проверить правильность ключа </td>
        </tr>
    </table>
</h3>


<h2 align = "center"> Link repositories <h2>
<h3>
    <table align = "center"> 
        <tr>
            <th> Command name </th>
            <th> Description </th>
        </tr>
        <tr>
            <td> cd «директория» </td>
            <td> Переход в директорию локального репозитория </td>
        <tr>
        <tr>
            <td>  git remote add origin «сыылка на удаленный репозиторий» </td>
            <td> Привязать удаленный репозиторий к локальному </td>
        </tr>
        <tr>
            <td> git remote -v </td>
            <td>  Проверка связи с удаленным репозиторием </td>
        </tr>
        <tr>
            <td> clip < ~/.ssh/id_ed25519.pub  </td>
            <td> Скопировать публичный SSH-ключ в буфер обмена </td>
        </tr>
        <tr>
            <td> ssh -T git@github.com </td>
            <td> Проверить правильность ключа </td>
        </tr>
    </table>
</h3>
