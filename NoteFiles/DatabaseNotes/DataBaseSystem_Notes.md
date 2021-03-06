>> DataBase Learning Notes

1. DB/DBMS/SQL 三者之间的关系
2. SQL语言基本适用于所有的数据库软件，但是每个数据库软件有部分属于自己特殊的SQL语言
3. 数据是先放入表中，表再放入到数据库中，一个数据库有很多个表，每个表对应一个名称，用来标识自己，表名具有唯一性
4. 表具有一些特性，这些特性决定了数据在表中是如何存储，类似**面对对象编程语言中类**的定义；表由列组成，也被称之为字段，所有的表是由一个或者多个字段组成，每个字段类似于类的一个属性
5. cmd命令行登录MySQL语句： 
>> mysql -h localhost -P 3306 -u root -p ***

<b>（分别表示host/端口号/用户名/密码，其中前两个参数可选）</b>

###+++常见命令+++（末尾记得加上分号）
>> show databases;  **查看当前所有的数据库**

>> use 库名; **打开指定的库**

>> show tables;    **查看当前库的所有表**
>> show tables from 库名; **查看其他库的所有表**

>> create table 表名(   **创建表**
>> 列名 列类型
>> 列名 列类型
>>)

>> desc 表名    **查看表结构**

>> select version();    **查看数据库版本**

### 语法规范
1. 不区分大小写，但是建议**关键字大写，表名、列名小写**

2. 每条命令用分号结尾，或者\g结尾

3. 每条命令根据需要，可以进行缩进或者换行
例如：SELECT 
        *
        FROM
        StuInfo;    # 表名

4. 注释
    单行注释： #注释文字
    单行注释： -- 注释文字，有个空格
    多行注释：/* 注释文字 */

+ DQL语言 ==> Data Query Language 数据查询语言
+ DML语言 ==> 数据操作语言
+ DDL语言 ==> 数据定义语言
+ TCL语言 ==> 事务控制语言
