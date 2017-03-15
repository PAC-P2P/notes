---
title: MPI 笔记
date: 2017-03-13 2017-03-13 06:48:35
tags: MPI
categories: Notes

---

MPI的笔记。

<!-- more --> 

## Concept

MPI(Massage Passing Interface):
消息传递函数库的标准规范，由MPI论坛开发，支持Fortran和C。


## Demo

简单的MPI并行程序Hello：

    #include <stdio.h>
    #include "mpi.h"
    
    main(int argc, char *argv[]){
        MPI_Init(&argc, &argv);     //MPI的初始化
        printf("Hello, world!\n");
        MPI_Finalize();
    }
    