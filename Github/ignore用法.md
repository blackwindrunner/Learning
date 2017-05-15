1. \#为注释   
2. 可以使用shell所使用的正则表达式来进行模式匹配   
3. 匹配模式最后跟"/"说明要忽略的是目录
4. 使用！取反（例如目录中包含  test.a，并且gitignore文件中包含  *.[oa]，如果在文件中加入 ！test.a   表明忽略除test.a文件以外的后缀名为.a或者.o的文件）

***

用法        |说明
--------- | -------------------
a.jpg		|显示指定忽略a.jpg文件
*.txt     |忽略所有以.txt结尾的文件
!name.txt |但不包括name.txt
build/    |会忽略build/目录下的文件
doc/*.txt| 会忽略doc/a.txt但不会忽略doc/files/a.txt
*.[oa]		|忽略后缀为.o和.a的文件


> 在add到缓冲区之前才可以使用.gitignore文件来忽略，如果已经add到缓冲区的文件，是无法忽略的。当通过git status查看文件状态的时候，
是不会看到已经在.gitignore文件中忽略的文件的

