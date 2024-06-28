# 如何永久修改Linux的open files数量

1.使用root用户编辑/etc/security/limits.conf

vim /etc/security/limits.conf

2.添加如下内容

\* soft nofile 65536

\*hard nofile 65536

![image-20240628113132609](https://raw.githubusercontent.com/program-keep/program-keep.github.io/main/img/2024-06-28/image-20240628113132609.png)

3.保存

4.重新登录

5.验证

ulimit -a 

![image-20240628113212023](https://raw.githubusercontent.com/program-keep/program-keep.github.io/main/img/2024-06-28/image-20240628113212023.png)

证明已修改成功

