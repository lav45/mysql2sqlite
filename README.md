mysql2sqlite
============

Sourse repository:
https://gist.github.com/esperlu/943776

Usage
============
copy paste this in a file, say: mysql2sqlite.sh file

make it executable:
```bash
$ chmod +x mysql2sqlite.sh
```
run it 
```bash
$ ./mysql2sqlite.sh -u MyUserName -pMySecretPassWord myDbase | sqlite3 database.sqlite
```
If you only need to create the table structures without data:
```bash
$ ./mysql2sqlite.sh --no-data -u MyUserName -pMySecretPassWord myDbase | sqlite3 database.sqlite
```