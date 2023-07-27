# raspberrypi_python

1 install vim/ ctags/ taglist

1.1 下载taglist_46.zip

1.2 如果没有~/.vim，那么 mkdir ~/.vim

1.3 将taglist_46.zip解压至 ~/.vim      unzip -o -d ./ /hisi/taglist_46.zip 

1.4 cd ~/.vim/doc

1.5 sudo apt-get install exuberant-ctags

1.6 vim进入编辑

1.7 (esc):helptags .     不要忘了点 " . "

1.8 (esc)：q退出vim编辑

1.9 which ctags   记显示的路径为 A

1.10  vim ~/.vimrc

1.11 加入以下三行

let Tlist_Show_One_File=1     "不同时显示多个文件的tag，只显示当前文件的    
let Tlist_Exit_OnlyWindow=1   "如果taglist窗口是最后一个窗口，则退出vim   
let Tlist_Ctags_Cmd="/usr/bin/ctags" "将taglist与ctags关联  ，注意改为路径 A

1.11 :wq 退出保存



2使用 vim 进入 （esc ）:Tlist (退出同样命令)

Ctrl+ww 切换左右窗口
