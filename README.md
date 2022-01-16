# XML
21. Создать внешний репозиторий c названием XML.
 GitHub > Repositories > New > XML
 22. Клонировать репозиторий XML на локальный компьютер.
 git clone 
 23. Внутри локального XML создать файл “new.xml”.
 cat > new.xml
 <?xml version="1.0" encoding="UTF-8" ?>
<root>
  <employeeID>1</employeeID>
  <name>Bill</name>
  <salary>56000</salary>
  <married>true</married>
</root>
 24. Добавить файл под гит.
 git add new.xml
 25. Закоммитить файл.
 git commit -m "new.xml adding for the first time"
 26. Отправить файл на внешний GitHub репозиторий.
 git push
 27. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
 vim new.xml
 <?xml version="1.0" encoding="UTF-8" ?>
 <root>
  <employeeID>1</employeeID>
  <name>Bill</name>
  <salary>56000</salary>
  <married>true</married>
  <employeeID>2</employeeID>
  <name>Olli</name>
  <salary>1000000</salary>
  <married>true</married>
  <age>27</age>
  <animals>1</animals>
 </root>
 /save and exit - :wq
 28. Отправить изменения на внешний репозиторий.
 git commit -am "add my employee2 information"
 git push
 29. Создать файл preferences.xml
 touch preferences.xml
 30. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.
 vim preferences.xml
 <?xml version="1.0" encoding="UTF-8" ?>
 <root>
  <fav_movie>The_Irony_of_Fate</fav_movie>
  <fav_serial>Friends_EN</fav_serial>
  <fav_food>vegetarian_dishes</fav_food>
  <fav_season>summer</fav_season>
  <fav_country>Iceland</fav_country>
 </root>
 31. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML
 touch skills.xml
 vim skills.xml
 <?xml version="1.0" encoding="UTF-8" ?>
 <root>
  <row>GitBash_Terminal</row>
  <row>GitHub</row>
  <row>API</row>
  <row>SQL</row>
  <row>Jmeter</row>
  <row>HTTPmethods</row>
  <row>JSON</row>
  <row>XML</row>
  <row>Charles</row>
  <row>Fidler</row>
  <row>VPN</row>
  <row>iOS_with_X-code</row>
  <row>Android_Studio</row>
  <row>PostgresDB</row>
  <row>Redis</row>
  <row>Python</row>
 </root>
 32. Сделать коммит в одну строку.
 git commit -a 
 add comment in vim window: add both xml files with preferences and skills
 33. Отправить сразу 2 файла на внешний репозиторий.
 git push
 34. На веб интерфейсе создать файл bug_report.xml.
 XML > Add file > Create new file > XML/bug_report.xml
 <?xml version="1.0" encoding="UTF-8" ?>
 <root>
  <id>1</id>
  <title>Chat - User cannot rename group conversation</title>
 </root>
 35. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 Comment for commit: add bug_report with bug report id information
 36. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
 Click bug_report.xml > edit 
 <?xml version="1.0" encoding="UTF-8" ?>
 <root>
  <id>1</id>
  <title>Chat - User cannot rename group conversation</title>
  <Type>Bug</Type>
  <Priority>Medium</Priority>
  <Affects_Version>None</Affects_Version>
  <Component>None</Component>
  <Labels>None</Labels>
  <Sprint>S22</Sprint>
  <Description>Steps_to_reproduce</Description>
  <1>Log in</1>
  <2>Open chat dialog</2>
  <3>Click on the Setting button</3>
  <4>Add user</4>
  <5>Add user to a group conversation</5>
  <6>Try to rename this group conversation</6>
  <Expected_result>User can rename group conversation</Expected_result>
  <Actual_result>Rename conversation button is disabled</Actual_result>
 </root>
 37. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
 Comment for commit: Update bug_report.xml
 38. Синхронизировать внешний и локальный репозиторий XML
 git fetch - проверка обновлений на внешнем репозитории
 git pull - синхронизация
