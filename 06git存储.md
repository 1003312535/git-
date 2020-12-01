在工作到一半不想提交，要切换到其他分支开发怎么搞

默认没有提交时不能切换分支的

#### 存储

stash 将未完成的修改保存到一个栈上

```js
git stash  #存储当前的
git stash list # 查看存储 
git stash apply #如果不指定存储的话 git 默认去除最新的
git stash pop #来应用储藏然后立即从栈上扔掉它
git stash drop #加上将要移出的储藏的名字来移出它
```

