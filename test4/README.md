# test4
1.创建用户study1<br>
如图：<br>
![t4](work4/1.png)<br><br>
ALTER USER STUDY QUOTA UNLIMITED ON USERS;<br>
ALTER USER STUDY QUOTA UNLIMITED ON USERS02;<br>
ALTER USER STUDY ACCOUNT UNLOCK;<br>

-- ROLES<br>
GRANT "CONNECT" TO STUDY WITH ADMIN OPTION;<br>
GRANT "RESOURCE" TO STUDY WITH ADMIN OPTION;<br>
ALTER USER STUDY DEFAULT ROLE "CONNECT","RESOURCE";<br>

-- SYSTEM PRIVILEGES<br>
GRANT CREATE VIEW TO STUDY WITH ADMIN OPTION;<br>
如图：<br>
![t4](work4/2.png)<br><br>
--删除表和序列
--删除表的同时会一起删除主外键、触发器、程序包。<br>
如图：<br>
![t4](work4/3.png)<br><br>
--  DDL for Table DEPARTMENTS<br>
如图：
![t4](work4/4.png)<br><br>
-创建3个触发器<br>
如图：
![t4](work4/5.png)<br><br>
--  DDL for Trigger ORDER_DETAILS_ROW_TRIG<br>
如图：![t4](work4/6.png)<br><br>
--插入DEPARTMENTS，EMPLOYEES数据<br>
如图：![t4](work4/7.png)<br><br>
递归查询某个员工及其所有下属，子下属员工。<br>
如图：![t4](work4/8.png)<br><br>
--查看数据文件的使用情况<br>
如图：![t4](work4/9.png)<br><br>