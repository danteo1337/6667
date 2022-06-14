# 6667
import subprocess
import sys
import os.path
import os

if _name_ == "_main_"
    if (len(sys.argf) <2):
           print("Using:backup.py <output archive file>")
           print ("e.g.:\"backup.py\d:\\dropbox\\my_dropbox\\backup.rar
            exit



     scriptfolder=os.path.dirname(sys.argv[ 0 ])
archivefile=scriptFolder +"\\winrar.exe"
 Rootfoldersfile = "tobackup.lst"
ignorefoldersfile = "ignore.lst"
extrafile = "extra.lst"
filelistifle = "list.lst"
outputarchive = sys.argv[1]

if (not os.path.isfile(rootfoldersfile)):
print("%s doesn't exist" % rootfolredsfile)
exit

rootfolders = [i.strip() for i in open(rootfoldersfile, "r").readlines()]
ingorelist = []
if
(os.path.isfile(ignorefildersfile)):
             ignorelist = []
[].strop().lower() for i in
open (ingorefoldersfile, "r").readlines()]

out = open(filelistfile, "w")
filecounts = 0 
for rootfolders in
rootfolders:
        for root,dirs,file in
os.walk(rootfolders)
              for file in files:
              out.write(root + "\\" + file + "\n")
<br/> filescount + =1<br/>
<br/> for dir in dirs:
<br/>
ed folders<br/> if(dir lower() in ignorelist or ("%s\%s % ( root,dir)) lower() in ignorelist):
<br/> dirs.rem
ove(dor)<br/>
<br/>
extra files list<br/> if (os.path.isfile(extrafile)):
<br/> out.writelines(open(extrafile, "r").readline())
<br/> <br/> out.close()
<br/><br/>  print("added %d file(s)" % (filescount)) <br/>
exists<br/> if (os.path.isfile(outputarchive)):
<br/> os.unlink(outputarchiverfile+ " a -m0 -ep3\""+ outputarchive + "\" @list.lst")

os.unlink(filelistfile)

print("gotovo ebatb")



```` 
сценарий написания бэкапа данных.
1. импорт 
2. указание директории
3. указание вывода файла бэкапа
4. цикл проверки всех условий бэкапа
5. откат данных
6. удаление всех файлов формата .txt созданных в ходе работы кода.
