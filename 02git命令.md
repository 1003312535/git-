全局配置初始化

```nginx
git config --global user.name 'ren'
git config --global user.email '100'
git list
git config  user.name 'ren' # 配置到本地文件中
git config user.email '100' # 配置到本地文件中
```

初始化项目

```nginx
git init
```

查看项目的**完整历史分支**

```js
git log --oneline --decorate --graph --all
git log --pretty=oneline #哈希值是完整的 显示简要日志信息
```

给上面命令**起别名**(注意双引号)

```js
git config --global alias.别名 “git log --oneline --decorate --graph --all”
```

li 

```linux
q! #强制退出
vim 修改内容
cat 查看内容
ll 查看当前目录中的文件和文件夹
echo 'new v1' > next.txt  创建文件
rm 删除操作
mv 换名字
```

```js
git commit
```

-a git 会把已经跟踪的文件暂存起来并且提交

```js
git commit -a -m ''
```

查看提交对象记录

```js
git log
git log --oneline 
```

git 删除 重命名 操作

```js
git rm 删除的文件 -----等价于（rm 文件；git add ./)
git mv 老文件     ------等价于（mv 新文件 ；rm 旧文件；git add ./）
```

#### git diff

```js
git diff  查看为暂存的修改
git diff cache 查看为提交的暂存
```

如果列表中项目的位置会动态改变或者有新的项目添加到列表中，并且希望列表中的项目保持自己的特征和状态（如 [input](https://developers.weixin.qq.com/miniprogram/dev/component/input.html) 中的输入内容，[switch](https://developers.weixin.qq.com/miniprogram/dev/component/switch.html) 的选中状态），需要使用 `wx:key` 来指定列表中项目的唯一的标识符。

`wx:key` 的值以两种形式提供

1. 字符串，代表在 for 循环的 array 中 item 的某个 property，该 property 的值需要是列表中唯一的字符串或数字，且不能动态改变。
2. 保留关键字 `*this` 代表在 for 循环中的 item 本身，这种表示需要 item 本身是一个唯一的字符串或者数字。

当数据改变触发渲染层重新渲染的时候，会校正带有 key 的组件，框架会确保他们被重新排序，而不是重新创建，以确保使组件保持自身的状态，并且提高列表渲染时的效率。

**如不提供 wx:key，会报一个 warning， 如果明确知道该列表是静态，或者不必关注其顺序，可以选择忽略。**