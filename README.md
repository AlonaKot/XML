# XML

1. Create an external repository with a name XML.
+ Open https://github.com/, Login in
+ Go to tab "Repositories"
+ Press "New"
+ Enter the name of the repository, make it public
+ Press "create repository"

 2. Clone repository XML to the local computer.
+ open GitBash in the folder where the repository will be stored
+ enter the command on the command line git clone + link to the repository we want to clone
 3. Create file inside local XML _new.xml_.
+ _cd XML_ - go to local repository
+ _cat > new.xml_
+ _ctrl + c_ - get out of editing
 4. Add file on git.
+ _git add new.xml_ - to add a particular file
+ _git add ._ - to add all files
 5. Commit the file.
+ _git commit -m "new file"_
 6. Submit a file to an external GitHub repository.
+ _git push_
 7. Edit file content _new.xml_ - write information about yourself (name, age, number of pets, future desired salary). Write everything in the format XML.
+ _vim new.xml_ 
+ press _"i"_
+ enter data
```
<?xml version="1.0"?>
	
<aboutme>
	<fullName> Alona Kot </fullName>
	<age> 25 </age>
	<pets> 1 </pets>
	<disiredSalary> 600$ </disiredSalary>
</aboutme>
```

+ press _"esc"_ enter _:wq_
 8. Push changes to an external repository.
+ _git add new.xml_ - add the changed file to git
+ _git commit -am "edit file"_ - commit changes
+ _git push_ - push modified file to external repository
 9. Create file _preferences.xml_
+ _vim preferences.xml_

 10. To file _preferences.xml_ dd information about your preferences (Favorite movie, favorite series, favorite food, favorite season, side you would like to visit) in the format XML.
+ press _"i"_
+ Enter text
```
<?xml version="1.0"?>

<myPreferences>
        <favoriteMovie> Indiana Jones </favoriteMovie>
        <favoriteSerias> Scrubs </favoriteSerias>
        <favoriteFood> Burgers </favoriteFood>
        <country> Switzerland </country>
</myPreferences>
```
+ press _"esc"_ enter _:wq_

 11. Create file _skills.xml_ add information about the skills that will be studied on the course in the format XML
 + _vim skills.xml_
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
+ press _"esc"_ enter _:wq_
	
 12. Make a commit in one line.
+ _git commit -m "new files"_
 
 13. Upload 2 files at once to an external repository.
 + _git add ._
 + _git push_
 
 14. Create a file on the web interface _bug_report.xml_.
 + In the repository XML press _"add file"_
 + Choose _"Create new file"_
 + Enter the file name
 
 15. Do Commit changes (save) changes on the web interface.
 
 + Press the button _"Commit new file"_
 
 16. Modify the file on the web interface _bug_report.xml_, add a bug report in the format XML.
 + Open file _bug_report.xml_ Select edit. Enter text
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
 17. Do Commit changes (save) changes on the web interface.
+ Press the button _Commit changes_.
 18. Synchronize external and local repository XML
+ _git pull_
