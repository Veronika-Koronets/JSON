# JSON
# Json. Git HW 1
# 1.Create an external repository called JSON.
Going to https://github.com/Veronika-Koronets?tab=repositories, then click "New", enter a name "Json", make it public and choose "Add a README file"
# 2. Cloning repository to local PC
Im going to my new repository. Click Code-->Local-->HTTP and copy this link.
Open GitBash on local PC.
Make folder "Json".

```sh
kv@kvPC MINGW64 /d
$ mkdir Json
$ cd Json
```
```sh
$ git clone https://github.com/Veronika-Koronets/JSON.git
Cloning into 'Json'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.
```
# 3. Create new.json file in the local repo

```sh
kv@kvPC MINGW64 /d/Json (main)
$ cat > new.json
```
> Now we see (main). 

# 4. Add a file for tracking
Use git add -->git status 
```
kv@kvPC MINGW64 /d/Json (main)
$ git add new.json

kv@kvPC MINGW64 /d/Json (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   new.json
``` 

## 5. Do commit file
```
kv@kvPC MINGW64 /d/Json (main)
$ git commit -m "new.json"
[main d943a0c] new.json
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.json
 ```
## 6. Send the file to remote repository
```
kv@kvPC MINGW64 /d/Json (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 278 bytes | 92.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/JSON.git
   017e004..d943a0c  main -> main
```


## 7. Edit the content of the “new.json” file - write information about yourself (full name, age, number of pets, future desired salary). Everything is written in JSON format.
.
```sh
kv@kvPC MINGW64 /d/Json (main)
$ vim new.json

kv@kvPC MINGW64 /d/Json (main)
$ cat new.json
{
       "person_name": "K. Veronika Gennadyevna" ,
       "person_age": "22" ,
       "number_of_pets": 1 ,
       "future_desired_salary": 1300
}
``` 
## 8. Send the changes to remote repository

```sh
kv@kvPC MINGW64 /d/Json (main)
$ git add new.json
warning: in the working copy of 'new.json', LF will be replaced by CRLF the next time Git touches it

kv@kvPC MINGW64 /d/Json (main)
$ git commit -m "changes new.json"
[main 84d4a0a] changes new.json
 1 file changed, 9 insertions(+)

kv@kvPC MINGW64 /d/Json (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 392 bytes | 130.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/JSON.git
   d943a0c..84d4a0a  main -> main
```

## 9. Create preferences.json file.
```
kv@kvPC MINGW64 /d/Json (main)
$ touch preferences.json
```

## 10. In the preferences.json file, add information about your preferences (Favorite movie, favorite series, favorite food, favorite season, side you would like to visit) in JSON format.

```
kv@kvPC MINGW64 /d/Json (main)
$ touch preferences.json

kv@kvPC MINGW64 /d/Json (main)
$ vim. preferences.json

kv@kvPC MINGW64 /d/Json (main)
$ cat. preferences.json
{
       "favourite_film":"Legally_Blonde" ,
       "favourite_series":"Blacklist"
       "favourite_food":"pizza" 
       "favourite_season":"spring"
       "Country_wish_to_visit":"Norway"
}
```

## 11. Create a file skills.json add information about the skills that will be studied in the course in JSON format.
```
kv@kvPC MINGW64 /d/Json (main)
$ vim skills.json

kv@kvPC MINGW64 /d/Json (main)
$ cat skills.json
{
"Git" ,
"Termianl" ,
"Postman" ,
"SQL" ,
"Charles" 
}
```

## 12. Send 2 files at once to an external repository
Use git add --> git commit -m --> git push
``` 
kv@kvPC MINGW64 /d/Json (main)
$ git add .
warning: in the working copy of 'preferences.json', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'skills.json', LF will be replaced by CRLF the next time Git touches it

kv@kvPC MINGW64 /d/Json (main)
$ git commit -m "add preferences and skills"
[main 0aae7ff] add preferences and skills
 2 files changed, 17 insertions(+)
 create mode 100644 preferences.json
 create mode 100644 skills.json

kv@kvPC MINGW64 /d/Json (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 527 bytes | 175.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Veronika-Koronets/JSON.git
   32a4819..0aae7ff  main -> main
```
## 13. Create a bug_report.json file on the web interface
## 14. Make Commit changes (save) changes on the web interface
## 15. Modify the bug_report.json file, add a bug report in JSON format on the web interface
## 16.Make Commit changes (save) changes on the web interface.
## 17. Synchronize external and local JSON repository

