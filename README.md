# graphrag-demo
graphrag使用案例

本项目是graphrag实践的案例项目，如果你拉取了我的代码，可以忽略`2`、`3`、`4`步骤，直接查询


## 运行步骤


### 1. 安装 GraphRAG

```
pip install graphrag
```

### 2. 初始化 GraphRAG

```
graphrag init --root ./ragtest
```

### 3. 修改配置

```
ragtest/settings.yaml
ragtest/.env
```

### 4. 运行索引管道构建知识图谱
```
graphrag index --root ./ragtest
```

### 5. 使用查询引擎

```
graphrag query --root ./ragtest --method global --query "你要查询的问题"
```

## 知识图谱可视化

### 1. 安装 `gephi`

安装软件`gephi`，[下载地址](https://gephi.org/users/download/)

### 2. 加载知识库

打开`gephi`，点击`打开图文件`，选择`ragtest/output/graph.graphml`, 为了方便你也可以直接使用`graphrag可视化.gephi`，这是作者调整过的现成图谱。

### 3. 调整知识图谱样式

![图片](/images/iShot_2025-05-07_09.20.11.png)

### 4. 输入文件

`gephi`的文件输出提供了多种选择，`图表`、`SVG`、`PNG`、`PDF`，
菜单位置`文件 - 输出`

![图片](/images/iShot_2025-05-07_09.16.44.png)