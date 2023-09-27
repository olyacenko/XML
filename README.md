# XML
 1. Create a remote repository named XML.
    - Go to GitHub account ;
    - click on the `new repository` button ;
    - enter Repository name "JSON" ;
    - click on the `Public` button ;
    - click `Add a README file` ;
    - click on `Create repository` button
 
 ----
2. Clone the XML repository to the local computer.
   - Go to the repository page ;
   - click on `Code` => `Local`=> ` SSH` => `Copy link` ;
   - on PC open terminal  => enter command `mkdir git_hw_1` => `cd git_hw_1` => `git clone git@github.com:olyacenko/XML.git`
```
dmitrijostalskij@MacBook-Pro-2 hw_ksendzov_courses % mkdir git_hw_1
dmitrijostalskij@MacBook-Pro-2 hw_ksendzov_courses % cd git_hw_1
dmitrijostalskij@MacBook-Pro-2 git_hw_1 % git clone git@github.com:olyacenko/XML.git
Cloning into 'XML'...
remote: Enumerating objects: 30, done.
remote: Counting objects: 100% (30/30), done.
remote: Compressing objects: 100% (25/25), done.
remote: Total 30 (delta 7), reused 8 (delta 0), pack-reused 0
Receiving objects: 100% (30/30), 8.41 KiB | 2.80 MiB/s, done.
Resolving deltas: 100% (7/7), done.
dmitrijostalskij@MacBook-Pro-2 git_hw_1 % 
```
 ----
3. Inside the local XML, create a "new.xml" file.
```
dmitrijostalskij@MacBook-Pro-2 git_hw_1 % cd XML 
dmitrijostalskij@MacBook-Pro-2 XML % touch new.xml
dmitrijostalskij@MacBook-Pro-2 XML %  
```
----
4. Add the file for tracking git.
```
dmitrijostalskij@MacBook-Pro-2 XML % git add new.xml  
```
----
5. Commit the file.
```
dmitrijostalskij@MacBook-Pro-2 XML % git commit -m "create new.xml"
[main cfdb003] create new.xml
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.xml
dmitrijostalskij@MacBook-Pro-2 XML % 
```
----
6. Send the file to the remote GitHub repository.
```
dmitrijostalskij@MacBook-Pro-2 XML % git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 279 bytes | 279.00 KiB/s, done.
Total 3 (delta 0), reused 1 (delta 0)
To github.com:olyacenko/XML.git
   cba65f8..cfdb003  main -> main
dmitrijostalskij@MacBook-Pro-2 XML % 
```
----
7. Edit the content of the file "new.xml" - write information about yourself (full name, age, number of pets, future desired salary). Write everything in XML format.
```
dmitrijostalskij@MacBook-Pro-2 XML % cat >> new.xml
<?xml version="1.0" encoding="UTF-8"?>
<xml>
<name>Olya</name>
<surname>Yatsenko</surname>
<age>29</age>
<pets />
<future_salary>500</future_salary>
</xml>
^C
dmitrijostalskij@MacBook-Pro-2 XML % 
```
----
8. Send the changes to the remote repository.
```
dmitrijostalskij@MacBook-Pro-2 XML % git add new.xml
dmitrijostalskij@MacBook-Pro-2 XML % git commit -m "add data to  new.xml"
[main 0e2d3b2] add data to  new.xml
 1 file changed, 8 insertions(+)
dmitrijostalskij@MacBook-Pro-2 XML % git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 405 bytes | 405.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To github.com:olyacenko/XML.git
   cfdb003..0e2d3b2  main -> main
dmitrijostalskij@MacBook-Pro-2 XML %  
```
----
9. Create "preferences.xml" file
```
dmitrijostalskij@MacBook-Pro-2 XML % touch preferences.xml 
```
----
10. In the preferences.xml file, add information about your preferences (Favorite movie, favorite show, favorite food, favorite time of year, party you would like to visit) in XML format.
```
dmitrijostalskij@MacBook-Pro-2 XML % cat >> preferences.xml
<?xml version="1.0" encoding="UTF-8"?>
<xml>
<favourite_movie>A beautiful mind</favourite_movie>
<favourite_series>The Sopranos</favourite_series>
<favourite_meal>meat</favourite_meal>
<favourite_time_of_year>summer</favourite_time_of_year>
<country_would_like_visit>Canada</country_would_like_visit>
</xml>
^C
dmitrijostalskij@MacBook-Pro-2 XML % 
```
----
11. Create skills.xml file and add information about skills that will be learned on the course in XML format.
```
dmitrijostalskij@MacBook-Pro-2 XML % cat > skills.xml
<?xml version="1.0" encoding="UTF-8"?>
<xml>
<Basic_theory>What is testing, bug reports, documentation, types, methods, testing directions, SDLC, STLC</Basic_theory>
<Client-server_architecture>Theory of client-server architecture</Client-server_architecture>
<HTTP>HTTP methods, HTTP server response codes, structures of HTTP inputs and responses</HTTP>
<JSON_XML>JSON, XML structure</JSON_XML>
<Postman>API testing via Postman, JS, API autotests</Postman>
<Logs>Removing and reading logs from an external server</Logs>
<Charles_Fiddler>Sniffing http web traffic and interception of traffic on iOS, Android</Charles_Fiddler>
<Dev_Tools>Web Dev Tools of Google Chrome, FireFox</Dev_Tools>
<VPN>How it works, why you need it, how to use it, tool options</VPN>
<Mobile_testing>Features of mobile testing, special cases</Mobile_testing>
<iOS_Android>Feature, guidelines</iOS_Android>
<Xcode>Building iOS applications</Xcode>
<Android_Studio>Building Android applications</Android_Studio>
<ADB>Android device mana<Proxy_vpn>Setting up on iOS and Android</Proxy_vpn>
<Terminal_Linux>copy, create, view, move files on servers without a graphical interface</Terminal_Linux>
<Basics_bash_scripting>Automation of routine tasks on the server</Basics_bash_scripting>
<SQL>basic operators: create, delete, delete, insert, select from, where, join</SQL>
<Postgres>database installation, configuration and use</Postgres>
<Redis>Non-relational database installation, configuration and use</Redis>
<Scrum>Theory of Development Methodology</Scrum>
</xml>
^C
dmitrijostalskij@MacBook-Pro-2 XML % 
```
----
12. Make the commit in one line.
```
dmitrijostalskij@MacBook-Pro-2 XML % git commit -am "add files preferences.xml and skills.xml "
[main bf57a37] add files preferences.xml and skills.xml
 2 files changed, 32 insertions(+)
 create mode 100644 preferences.xml
 create mode 100644 skills.xml
dmitrijostalskij@MacBook-Pro-2 XML % 
```
----
13. Send 2 files at once to the remote repository.
```
dmitrijostalskij@MacBook-Pro-2 XML % git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 1.29 KiB | 1.29 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0)
To github.com:olyacenko/XML.git
   0e2d3b2..bf57a37  main -> main
dmitrijostalskij@MacBook-Pro-2 XML % 
```
----
14. Create bug_report.xml file on the web interface.
    - go to the remote repository ;
    - click `Add file` button ;
    - `Create new file` ;
    - enter name of the file "bug_report.xml" ; 
-----
15. Make Commit changes (save) the changes on the web interface.
    - click `Commit changes` => enter the description "create bug_report.xml " ;
    - click `Commit directly to the main branch` ;
    - click `Commit changes` 
----
16. On the web interface, modify bug_report.json file, add bug report in XML format.
    - click on the file "bug_report.xml" ;
    - click `edit this file` ;
    - add data to the file
----
17. Make Commit changes (save) the changes on the web interface.
    - click `Commit changes` => enter the description "add data to bug_report.xml " ;
    - click `Commit directly to the main branch` ;
    - click `Commit changes`
----
18. Synchronize external and local XML repository.
```
dmitrijostalskij@MacBook-Pro-2 XML % git pull
remote: Enumerating objects: 7, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (5/5), done.
remote: Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), done.
From github.com:olyacenko/XML
   bf57a37..52e0a02  main       -> origin/main
Updating bf57a37..52e0a02
Fast-forward
 bug_report.xml | 21 +++++++++++++++++++++
 1 file changed, 21 insertions(+)
 create mode 100644 bug_report.xml
dmitrijostalskij@MacBook-Pro-2 XML % 
```










   
