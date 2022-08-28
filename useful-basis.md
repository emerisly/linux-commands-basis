
## Some Git
re-upload entire repo: ```git pull origin master --allow-unrelated-histories```  
fix uncommitted mistake: ```git reset```  
fix committed mistake: ```git revert $ID```  
uncommit all: ```git reset --soft HEAD^``` and then ```git reset```  
get lines of code: ```git ls-files | grep '\.py' | xargs wc -l```
ignore modified files: ```git update-index --assume-unchanged $DIR/FILE```  
refresh gitignore: ```git ls-files --deleted -z | git update-index --assume-unchanged -z --stdin```   
```
git init
git commit -m "first commit"
git branch -M master
git remote add origin https://github.com/emerisly/temp.git
# or git remote add origin git@github.com:emerisly/temp.git
git push -u origin master
``` 

-------------------------------------------------------------------

## Download

### download from google drive [link](https://stackoverflow.com/questions/25010369/wget-curl-large-file-from-google-drive)  
files: drive.google.com/file/d/$FILE_ID/view?usp=sharing   
folders: drive.google.com/drive/folders/$FILE_ID  
get file: ```gdown $FILE_ID```  
get folder: ```gdown –folder –id $FILE_ID```   

### Download using nohup, download on background
-c continue  
download: ```nohup wget -c $URL 2>&1 &```   


### Multi-thread download using aria2 [link](https://aria2.github.io/)
-x16 connections -s16 splits: ```aria2c -x16 -s16 $URL```

-------------------------------------------------------------------

## Show Progress Bar
for programs that takes long to run  
[tqdm](https://github.com/tqdm/tqdm)

-------------------------------------------------------------------

## Conda
activate: ```conda activate $ENV```  
show env: ```conda list```  

-------------------------------------------------------------------


## Vim
action           | command
---------------- | -----------
save and quit    |  ```wq```  
inset            | ```i```  
insert at cursor | ```a```  
search           | ```/pattern```
replace          | ```:%s/old/new/g```
wildcards        | ```.*```
number           | ```\d```
letter           | ```\w```

-------------------------------------------------------------------


## Shortcuts VSCode
clear terminal: ```ctrl + L```  
clear current cmd: ```ctrl + U``` 