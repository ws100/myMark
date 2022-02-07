# Git常用命令

![](https://git-scm.com/images/branching-illustration@2x.png)

## 初始化

### 打开GitBash

![image-20220207113450680](git.assets/image-20220207113450680.png)

### 查询git版本

```
git --version
```
### 清屏

```
clear
```

### 设置用户名和邮箱

```
git config --global user.name "ws"
git config --global user.email "1841657140@qq.com"
```

### 创建并进入文件夹

```
mkdir mark
cd mark
```

### 初始化操作

```
git init
```
#### **创建成功出现（master）**

![image-20220207114233130](git.assets/image-20220207114233130.png)



#### **新创建的文件**

![image-20220207114250703](git.assets/image-20220207114250703.png)

## add和commit命令

**文件和.git同一个目录**

![image-20220207114703275](git.assets/image-20220207114703275.png)

### 提交到暂存区

```
git add demo.txt
```

### 提交到本地库

```
git commit -m "这是一个文件"
```

- **-m 表示注释**

![image-20220207115042753](git.assets/image-20220207115042753.png)

### 注意

- **不放在本地仓库的文件，git不管理**
- **放在本地库中的文件，git也不管理，必须通过add，commit命令才可以使用git**

## status命令

```
git status
```

### 全部被管理时

![image-20220207115552418](git.assets/image-20220207115552418.png)

### 新建demo2（没有被管理）

![image-20220207115720945](git.assets/image-20220207115720945.png)

### 执行add命令后

![image-20220207115844243](git.assets/image-20220207115844243.png)

### 执行commit命令之后

![image-20220207120002656](git.assets/image-20220207120002656.png)

### 文件被修改

![image-20220207120234459](git.assets/image-20220207120234459.png)

## log命令

```
git log
```

### 显示日志

![image-20220207120530890](git.assets/image-20220207120530890.png)

### 分页效果（当日志过多时）

- 下一页：空格
- 上一页：b
- 尾页：显示END
- 退出：q

### 在一行内显示

```
git log --pretty=oneline
```

![image-20220207121022534](git.assets/image-20220207121022534.png)

```
git log --oneline
```

![image-20220207121114430](git.assets/image-20220207121114430.png)

### 显示带指针的日志

```
git reflog
```

![image-20220207121313434](git.assets/image-20220207121313434.png)

## reset命令

### 通过reflog查看日志（通过索引回退）

```
git reflog
```

![image-20220207121903515](git.assets/image-20220207121903515.png)

### reset命令回退

```
git reset --hard 7528a4e
```

### 再次查看reflog

![image-20220207122307235](git.assets/image-20220207122307235.png)

### 文件回到历史版本

![image-20220207122506238](git.assets/image-20220207122506238.png)

### hard，soft，mixed

#### hard

| **（更    改）** | **（更    改）** | **（更    改）** |
| :--------------: | :--------------: | :--------------: |
|    **工作区**    |    **暂存区**    |    **本地库**    |

#### mixed

|   **工作区**   | **（更    改）** | **（更    改）** |
| :------------: | :--------------: | :--------------: |
| **（未更改）** |    **暂存区**    |    **本地库**    |

#### soft

|   **工作区**   |   **暂存区**   | **（更    改）** |
| :------------: | :------------: | :--------------: |
| **（未更改）** | **（未更改）** |    **本地库**    |

## 删除与找回

### 删除工作区

```
rm test.txt
```

### 将删除操作同步到暂存区

```
git add test.txt
```

### 将删除操作同步到本地库

```
git commit -m "删除test.txt"
```

### 查看日志

![image-20220207123748314](git.assets/image-20220207123748314.png)

### 用reset命令找回

```
 git reset --hard 7528a4e
```

![image-20220207124113381](git.assets/image-20220207124113381.png)

### 找回缓存区的文件（reset第一个索引即可）

![image-20220207124527271](git.assets/image-20220207124527271.png)

## diff命令

### 比较工作区和暂存区的文件

#### 比较一个文件

```
git diff test2.txt
```

![image-20220207125212277](git.assets/image-20220207125212277.png)

#### 比较所有文件

```
git diff
```

![image-20220207125352584](git.assets/image-20220207125352584.png)

### 比较暂存区和本地库的文件

```
git diff HEAD test2.txt
```

![image-20220207125841225](git.assets/image-20220207125841225.png)

### 通过索引比较

```
git diff 43f655a test2.txt
```

![image-20220207130120495](git.assets/image-20220207130120495.png)

## 分支

### 示意图

![image-20220207130620991](git.assets/image-20220207130620991.png)

### 分支的好处

- **同时多个分支并行，提高开发效率**
- **一个分支失败不影响其他分支**

### 查看分支

```
git branch -v
```

![image-20220207131018386](git.assets/image-20220207131018386.png)

### 新建分支

```
git branch branch01
```

![image-20220207131202335](git.assets/image-20220207131202335.png)

### 切换分支

```
git checkout branch01
```

![image-20220207131508788](git.assets/image-20220207131508788.png)

### 合并分支

#### 合并命令（出现冲突）

```
git merge branch01
```

![image-20220207132640001](git.assets/image-20220207132640001.png)

#### 查看冲突

```
cat test3.txt
```

![image-20220207132814699](git.assets/image-20220207132814699.png)

#### 解决（修改后重新提交）

```
git add test3.txt
```

```
$ git commit -m "修改好了"
```

![image-20220207133610283](git.assets/image-20220207133610283.png)

# GitHub

![](https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fimg3.doubanio.com%2Fview%2Fnote%2Fl%2Fpublic%2Fp59835864.jpg&refer=http%3A%2F%2Fimg3.doubanio.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=jpeg?sec=1646805581&t=80fc8af4b3963ffe1de624a1c58240a8)

## 创建一个库

![image-20220207140935253](git.assets/image-20220207140935253.png)

## 将本地资源推送到远程库

### 远程库的地址

![image-20220207141120160](git.assets/image-20220207141120160.png)

### 将地址保存

```
 git remote add origin https://github.com/ws100/-.git
 git remote -v
```

![image-20220207141406257](git.assets/image-20220207141406257.png)

