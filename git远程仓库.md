配置一个远程仓库，并且起别名

```js
git remote add 别名 仓库地址
```

查看远程仓库跟多信息

```js
git remote show [仓库名]
```

重命名 别名

```js
git remote rename  旧 新
```

#### 显示远程仓库 别名 和 路径

```js
git remote -v 
```

第一次推送到远程分支上

```js
git push origin master
```



### 用户

#### 克隆远程仓库

```js
git clone 仓库地址
```

邀请成员

默认不是成员不能push 项目到仓库中

只能克隆

项目设置-->collaborators---->成员名 ---->复制邀请链接 发给对方 -----> 对方点击同意------->成为合作伙伴

## 远程跟踪分支

远程仓库中的叫远程分支、(master)

本地中的叫本地分支、(master)

远程仓库中的叫远程跟踪分支（taobao/master ，当推送到远程仓库时默认自动创建的 媒介）、

#### 从远程仓库拿数据

```js
git fetch 远程仓库名
```

默认会把最新项目拿到**远程跟踪分支上了**（taobao/master）

