# test2
1 以system登录到pdborcl，创建角色Xchaun和用户Xc，并授权和分配空间<br>
实验代码<br>
CREATE ROLE Xchaun;<br>
GRANT connect,resource,CREATE VIEW TO Xchaun;<br>
CREATE USER Xc IDENTIFIED BY 123 DEFAULT TABLESPACE users TEMPORARY TABLESPACE temp;<br>
ALTER USER Xc QUOTA 50M ON users;<br>
如图<br>
![t2](work2/01.png)<br><br>
结果如图：<br>
![t2](work2/02.png)<br><br>
2新用户Xc连接到pdborcl，创建表mytable和视图myview，插入数据，最后将myview的SELECT对象权限授予hr用户。<br><br>
实验代码如图：<br>
![t2](work2/03.png)<br><br>
结果如图：<br>
![t2](work2/04.png)<br><br>
