# Learn_Lua



## 概念

### 1. Lua
```sh
Lua is a powerful, efficient, lightweight, embeddable scripting language. It supports procedural programming, object-oriented programming, functional programming, data-driven programming, and data description.
```


### 2. LuaJIT
```sh
LuaJIT is a Just-In-Time Compiler (JIT) for the Lua programming language.
```


### 3. Lua虚拟机(VM)
```sh
- 分类：基于栈（Stack Base）、基于寄存器（Register Base）
- Dalvik是基于寄存器的虚拟机，Java、.NET CLR、Python、Ruby、Lua5.0之前的版本的虚拟机都是基于栈的虚拟机；从5.0版本开始，Lua的虚拟机改成了基于寄存器的虚拟机。
```

## 参考
- lua: http://www.lua.org/
- luajit: http://luajit.org/luajit.html
- tolua: http://webserver2.tecgraf.puc-rio.br/~celes/tolua/tolua-3.2.html
- tolua-runtime: https://github.com/topameng/tolua_runtime



## 安装
需要root权限
```sh
curl -R -O http://www.lua.org/ftp/lua-5.4.3.tar.gz
tar zxf lua-5.4.3.tar.gz
cd lua-5.4.3
make all test
make install
```

## 查看版本
```sh
➜  ~ lua -v
Lua 5.4.3  Copyright (C) 1994-2021 Lua.org, PUC-Rio
```

## 执行
- 方式一
```sh
➜  ~ lua
Lua 5.4.3  Copyright (C) 1994-2021 Lua.org, PUC-Rio
> print('hello world')
hello world
> os.exit() //退出，或者Ctrl + C
```

- 方式二
```sh
➜  ~ vi hello.lua
print("hello world")

➜  ~ lua hello.lua
hello world
```

- 方式三
```sh
➜  ~ lua
Lua 5.4.3  Copyright (C) 1994-2021 Lua.org, PUC-Rio
> dofile('hello.lua')
hello world
```


## 数据类型
```sh
Lua语言中有8种基本类型： 
- nil （空）
- boolean （布尔）
- number （数值）
- string （字符串）
- userdata（用户数据）
- function （函数）
- thread （线程）
- table （表）
```