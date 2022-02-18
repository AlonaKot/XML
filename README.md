# XML

1. Создать внешний репозиторий c названием XML.
+ Открыть https://github.com/, залогиниться 
+ Зайти во вкладку `Repositories`
+ Нажеть `New`
+ Ввести название репозитория, сделать его общедоступным
+ Нажать `create repository`

2. Клонировать репозиторий XML на локальный компьютер.
+ открыть GitBash в папке, где будет храниться репозиторий
+ в командную стороку ввести команду git clone + ссылка на репозиторий, который хотим клонировать
 3. Внутри локального XML создать файл “new.xml”.
+ `cd XML` - перейти в локальный репозиторий
+ `cat > new.xml`
+ `ctrl + c` - выйти из редактирования
 4. Добавить файл под гит.
+ `git add new.xml` - для добавления определенного файла
+ `git add .` - для добавления всех файлов
 5. Закоммитить файл.
+ `git commit -m "new file"`
 6. Отправить файл на внешний GitHub репозиторий.
+ `git push`
 7. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
+ `vim new.xml` 
+ нажать `i`
+ внести данные
```
<?xml version="1.0"?>
	
<aboutme>
	<fullName> Alona Kot </fullName>
	<age> 25 </age>
	<pets> 1 </pets>
	<disiredSalary> 600$ </disiredSalary>
</aboutme>
```
+ нажать `esc` ввести `:wq`
8. Отправить изменения на внешний репозиторий.
+ `git add new.xml` - добавить измененный файл под гит
+ `git commit -am "edit file"` - закомитить изменения
+ `git push` - отправить измененный файл на внешний реозиторий
9. Создать файл preferences.xml
+ `vim preferences.xml`
10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.
+ нажать `i` - для редактирования 
+ внести данные
```
<?xml version="1.0"?>

<myPreferences>
        <favoriteMovie> Indiana Jones </favoriteMovie>
        <favoriteSerias> Scrubs </favoriteSerias>
        <favoriteFood> Burgers </favoriteFood>
        <country> Switzerland </country>
</myPreferences>
```
+ нажать `esc` ввести `:wq`
11. Создать файл skills.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML
+ `vim skills.xml`
 ```
 <?xml version="1.0"?>
 
<hardsSkills>
		<skill> Basic theory </skill>
		<skill> Client-server architecture </skill>
		<skill> HTTP Server request methods </skill>
		<skill> HTTP Server responses codes </skill>
		<skill> Structures of requests and responses </skill>
		<skill> JSON, XML. Their structure </skill>
		<skill> API testing </skill>
		<skill> Removing and reading logs </skill>
		<skill> POSTMAN, FIDLER </skill>
		<skill> VPN </skill>
		<skill> Dev Tools for web browsers </skill>
		<skill> Mobile testing </skill>
		<skill> Feature iOS, Android, guidelines </skill>
		<skill> Building iOS Apps with Xcode </skill>
		<skill> Building Android Applications with Android Studio </skill>
		<skill> Interception of mobile traffic (sniffing) via CHARLES </skill>
		<skill> Proxy settings on iOS and Android </skill>
		<skill> Terminal Linux Ubuntu. Copying, creating, viewing, moving files on servers without a graphical interface </skill>
		<skill> Simple bash scripting, automation of routine tasks on the server </skill>
		<skill> Access to remote servers </skill>
		<skill> SQL fundamentals (Create, Delete, Drop, Insert Into, Select, From, Where, Join </skill>
		<skill> GIT </skill>
		<skill> JMETER </skill>
		<skill> Scrum Development Methodology </skill>
		<skill> Python. Creation of own client-server application </skill>
</hardsSkills>	
```
+ нажать `esc` ввести `:wq`
12. Сделать коммит в одну строку.
+ `git commit -m "new files"`
13. Отправить сразу 2 файла на внешний репозиторий.
+ `git add .`
+ `git push`
14. На веб интерфейсе создать файл bug_report.xml.
+ В репозитории XML нажать `add file`
+ Выбрать `Create new file`
+ Вести название файла
15. Сделать Commit changes (сохранить) изменения на веб интерфейсе. 
+ Нажать кнопку `Commit new file`
16. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
+ Открыть файл bug_report.xml Выбрать редактирование. Ввести текст
```
<?xml version="1.0"?>

<bugReport>
        <Summary> Displaying a characteristic associated with a deleted group </Summary>
        <Priority> Major </Priority>
        <Severity> Midle </Severity>
        <Status> To do </Status>
        <Environment> Desktop, Windows10 x64, Chrome97 </Environment>
        <Descriprion>
                   <Precondition>
                              <one> Authorization in your personal account </one>
                              <two> Switch the mode to store management (store_url/admin/home) </two>
                              <three> In the sidebar, expand the 'Catalog' list </three>
                              <four> The submenu 'Characteristics' is open </four>
                              <five> Characteristics &quot;Test&quot;, &quot;Test 1&quot;, &quot;Test 2&quot; are included in the group of characteristics &quot;Overall dimensions&quot; </five>
                              <six> The subgroup &quot;Groups of characteristics&quot; is opened </six>
                    </Precondition>
                    <Steps to Reproduce>
                              <one> Click on the kebab menu next to the group 'Dimensions'</one>
                              <two> Select the &quot;Delete&quot; menu in the kebab </two>
                    </Steps to Reproduce>
                    <Actual Result>
                              <one> Group deleted </one>
                              <two> When switching to the &quot;Characteristics&quot; tab, the characteristics &quot;Test&quot;, &quot;Test 1&quot;, &quot;Test 2&quot; are displayed with binding to the deleted group </two>
                    </Actual Result>     
                    <Expected Result>
                              <one> Group deleted </one>
                              <two> When switching to the &quot;Characteristics&quot; tab, the characteristics &quot;Test&quot;, &quot;Test 1&quot;, &quot;Test 2&quot; are displayed without binding to the remote group </two>
                    </Expected Result>
        </Descriprion>
        <Attachment xmlns:xlink="https://drive.google.com/file/d/1KAg5XKZQIQC6zYaOxrDbs2ng1LBuOxcz/view?usp=sharing"> Attachment </Attachment>
        <Assignee/>
        <Reporter> Alona Kot </Reporter>
</bugReport> 
```
17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
+ Нажать кнопку `Commit changes`
18. Синхронизировать внешний и локальный репозиторий XML
+ `git pull`
