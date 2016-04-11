﻿libuv source analysis - Say it from libuv  
libuv源码分析 - 从libuv说开来

Wiki: https://github.com/paulran/libuv-source-analysis/wiki  
Website: http://paulran.github.io/libuv-source-analysis


The project objectives:  
项目目标：  
1. Be able to use libuv in future projects.  
1. 在将来项目中能够使用libuv。  
2. Sum up the relevant knowledge.  
2. 总结相关的知识。  


The analytical methods:  
分析方法：  
1. Designer angle: Ask why the design is like this? Are there any other designs?  
1. 设计者角度：多问为什么这么设计？是否还有其它设计？  
2. User perspective: what interfaces are provided, what is the use of the process, the use of test examples of debugging and testing, to understand the meaning of the data structure.  
2. 用户角度：提供了哪些接口，使用流程是什么，使用测试例子调试测试，弄清数据结构的含义。  


libuv version 1.8.0 (Stable)  
```
libuv-1.8.0 files for Linux
├── include
│   ├── pthread-fixes.h
│   ├── tree.h
│   ├── uv-errno.h
│   ├── uv.h
│   ├── uv-linux.h
│   ├── uv-threadpool.h
│   ├── uv-unix.h
│   └── uv-version.h
└── src
    ├── fs-poll.c
    ├── heap-inl.h
    ├── inet.c
    ├── queue.h
    ├── threadpool.c
    ├── unix
    │   ├── async.c
    │   ├── atomic-ops.h
    │   ├── core.c
    │   ├── dl.c
    │   ├── fs.c
    │   ├── getaddrinfo.c
    │   ├── getnameinfo.c
    │   ├── internal.h
    │   ├── linux-core.c
    │   ├── linux-inotify.c
    │   ├── linux-syscalls.c
    │   ├── linux-syscalls.h
    │   ├── loop.c
    │   ├── loop-watcher.c
    │   ├── pipe.c
    │   ├── poll.c
    │   ├── process.c
    │   ├── proctitle.c
    │   ├── pthread-fixes.c
    │   ├── signal.c
    │   ├── spinlock.h
    │   ├── stream.c
    │   ├── tcp.c
    │   ├── thread.c
    │   ├── timer.c
    │   ├── tty.c
    │   └── udp.c
    ├── uv-common.c
    ├── uv-common.h
    └── version.c
```