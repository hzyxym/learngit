# learngit
廖雪峰demo

1.修改commit注释参考 https://blog.csdn.net/lxf0613050210/article/details/52525083
首先 使用 git commit --amend 命令，（修改最近一次提交的注释信息），会进入到vim 编辑器

然后 你会发现编辑器里你怎么输入都没反应，这是因为vim处在不可编辑状态，按下字母键 c，此时进入编辑状态，可以开始修改注释信息了

在然后 你会发现你怎么都退出不了，回到shell了，然后操作如下： ESC  --》 退出编辑状态；接着 连续按两次大写字母键 Z，接着你会惊喜的发现，终于保存好退出来了！
1.git rebase -i HEAD~10 修改一条 pick -> edit
2.git commit --amend 修改注释
3.git rebase --continue

2.还原误删的分支：
  首先想办法把被误删的分支的代码https://blog.csdn.net/fdipzone/article/details/50616386?utm_source=blogxgwz7
  最后：git push origin dev-5.1.0
