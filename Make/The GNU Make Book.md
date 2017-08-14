#The GNU Make Book
#####    by John Graham-cumming

# 第1章 基本知识回顾

本章涵盖了可以认为是GNU make基础知识的材料，但是也强调了一些常常被误解的功能，澄清了一些GNU make关注的部分。此外，还介绍了GNU make版本`3.79.1`、`3.81`、`3.83`和`4.0`之间的不同之处。如果你还在使用`3.79.1`之前的版本的话，那么你可能应该升级了。

本章决不能替代官方**GNU make手册(GNU make manual)**，我强烈建议你拥有一份，你可以在[http://www.gnu.org/make/manual](http://www.gnu.org/make/manual)找到它。

# 在GNU make中使用环境变量

当GNU make启动以后，在环境中设置的任何变量都可以作为Makefile中的一个GNU make变量。例如，考虑下面的Makefile：
***
$(info $FOO)
***
