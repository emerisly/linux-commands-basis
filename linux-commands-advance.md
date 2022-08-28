You don't need to remember all commands. It is a good idea to keep your own cheat sheet!  
Check out the commands below and add it to your personal cheat sheet if you find it useful.  
You might need to install packages for some of the commands such as nvitop. Google is your friend.

## Linux
- space availability: ```df -h```  
- gpu availability: ```watch -n 1 -d nvidia-smi```  
- gpu availability: ```nvitop```  
- nvidia and CUDA info: ```nvidia-smi```  
- get id_rsa: ```cat ~/.ssh/id_rsa.pub```  
- print working directory: ```pwd```  
- get pwd in folder: ``` open `pwd` ```  
- give access to other servers: ```chmod 777 -R *```  
- mounted to server: ```/mnt/$SERVER/```  
- files size in dir: ```du -sh *```  
- files access in dir: ```ls -alh```  
- dir in tree: ```tree -d $DIR```  
- dir in tree with depth: ```tree -d $DIR -L $NUM```  
- move or download dir : ```scp -r $DIR $SERVER:$DEST_DIR/```  
- view threads of a process: ```ps - ef | grep $NAME```   
- unzip 7z: ```7za e myfiles.7z```  
- unzip tar.gz: ```tar -xvf archive.tar.gz```  
- count folders/files in this dir: ```ls | wc -l```  
- count files in dir: ```ls -R | wc -l``` or ```du -a | cut -d/ -f2 | sort | uniq -c | sort -nr```  
- count files with type in dir: ```find . -name "*.jpg" | wc -l```  
- get PID jupyter notebook: ```lsof -n -i4TCP:$PORT```  
- kill PID: ```kill -9 $PID```  
- list 4 files in dir: ```ls -U | head -4```  
- run python on nohup: ```nohup python3 $FILE &```  
- nohup with output: ```nohup python3 -u $FILE.py > nohup0.out 2>&1 &```
- create shortcutes: ```ln -s $DEST_DIR $SHORTCUT_DIR```   
- tmux session: ```tmux a -t $SESSION```  