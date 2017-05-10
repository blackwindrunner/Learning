# 



\# 为注释

用法        |说明
--------- | -------------------
*.txt     |忽略所有以.txt结尾的文件
!name.txt |但不包括name.txt
build/    |会忽略build/目录下的文件
doc/*.txt| 会忽略doc/a.txt但不会忽略doc/files/a.txt


> 在add到缓冲区之前才可以使用.gitignore文件来忽略，如果已经add到缓冲区的文件，是无法忽略的。当通过git status查看文件状态的时候，
是不会看到已经在.gitignore文件中忽略的文件的
