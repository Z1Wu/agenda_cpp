# Agenda

## 如何运行

> 运行环境： win10 + mingw32

1. 使用 makefile 编译并构建整个系统

``` bash
# 移动到文件根目录下，执行make
# 详细构建流程查看根目录下的 MakeFile 的内容

make
```
2. 运行构建生成的

``` bash
./bin/Agenda.exe
```

3. 测试结束之后，清除生成的文件

``` bash
make clean
```

## 系统简要架构

这个系统的设计使用了`三层架构(3 tier architecture)`的设计方式，分为以下三个层

- UI layer: 主要是指与用户交互的界面，在这个程序是一个简单的命令行界面。

- Service layer: 业务逻辑层，用户交互层和存储层之间的桥梁，实现具体的业务逻辑，包括验证、计算、业务规则等等。

- Entity layer: 数据访问层/数据存储层，实现数据的持久化。

// UML 类图(todo)

## 程序功能

详见 [doc](./doc/AgendaRequirement.md) 


