---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
rise:
  start_slideshow_at: beginning

kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# 作业 #

作业一：请指出paddle在初始位置的四个顶点坐标。

作业二：球拍的初始位置如图所示，请问paddle_x与paddle_y的初始值应该如何修改？

作业三：小球目前与边框发生弹性碰撞，如果要求与球拍的上底面也可以发生碰撞，程序应该如何修改？应该如何检测小球与上底面发生了碰撞？碰撞后速度会如何变化？

请描述你的设计逻辑，不需要写代码。

![paddle_pos](paddle_pos.png)

作业四：设计游戏

分为三个难度，你可以任选一个难度来做：

A（满分60）: 完成作业二的设计，不需要小球与球拍发生碰撞。

B（满分80）: 在A的基础上完成作业三的设计，要求小球接触到球拍上底面的时候，会发生弹性碰撞。

C (满分100)：在B的基础上，引入游戏规则：当小球碰到下边框的时候，游戏窗口自动关闭。


## 提交 ##

其中作业一、二、三提交在homework.txt里，作业四提交在main.py中。

截止时间：周三晚上10点