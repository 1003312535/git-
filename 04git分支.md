分支就是一个指针，在提交对象的前面

HEAD文件和 refs 文件夹

### refs 目录存储之间数据的提交对象的指针

* refs中有对应的分支文件，文件中存储的 指针指向的提交对象的哈希值

创建分支

```
git branch 查看
git branch aaa 创建
git branch -D aaa 删除
git branch -v 查看分支的最后一次提交
git branch aaa hash值  创建一个分支并且把这个分支指向一个提交对象	
git branch -merged
```

切换分支

```js
git checkout aaa
```



### HEAD 文件只是目前检出的分支 

* 当前所在那个分支上
* 分支是一个指针指向提交对象，，每次提交时，head带着当前的分支向前移动**指向新的提交对象**

#### **分支的本质**

就是一个指向提交对象上的指针

head 是一个指针 ，默认指向master分支

切换分支就是让HEAD指向不同的分支



