# Films List

> Web 第三次作业

## 作业完成情况

### 必选项

- [x] 将 `films_all.json` 写入数据库
- [x] 服务端访问数据库，客户端访问服务端接口，完成第二次作业实现的功能
- [x] 部署到线上服务器，提供访问地址

### 访问地址

http://srszd.top:5678

## 项目报告

### 项目地址

<https://github.com/ChenCyl/film-list>

### 技术栈

- 前端：Vue
- 后端：Node.js
- 数据库：MongoDB
- 部署：Docker Compose 

### 功能介绍

#### 1. 数据统计及可视化

电影详情页中，电影的评分分布情况涉及到数据的可视化，我选用 **D3** 作为可视化的工具，绘制了条形图来呈现评分的分布情况。

#### 2. 搜索功能

实现基于**片名、演员名、导演名、影片类型**的搜索功能。

- [x] 分页

- [x] 电影详情页
- [x] 数据统计及可视化

### 针对第二次作业的优化

- [ ] 在后端增加通过 ID 获得电影详情页的接口
- [ ] 增加加载动画
- [ ] Home 按钮

---

```
rsync av -e ssh --exclude='node_modules' film-list root@47.102.112.138:/mnt/
```

-a ：递归到目录，即复制所有文件和子目录。另外，打开归档模式和所有其他选项（相当于 -rlptgoD）
-v ：详细输出
-e ssh ：使用 ssh 作为远程 shell，这样所有的东西都被加密
--exclude='*.out' ：排除匹配模式的文件，例如 *.out 或 *.c 等。