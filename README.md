# Learn-SQL
##SQL 语句声明
```
CREATE TABLE table_name (
    column_1 data_type, 
    column_2 data_type, 
    column_3 data_type
  );
```

- SQL 语句以 `;`结束
- `CREATE TABLE`是一个分句，也可以被称为SQL中的指令，在 SQL 中会执行特定的任务，所有字母大写
- `table_name` 是指令所操作的表格名称
- `(column_1 data_type, column_2 data_type, column_3 data_type)` 是参数，参数是一个`columns(列)`,` data types（数据类型）`,`values（值）`的集合，作为参数传递给指令
- 书写的时候换不换行无关紧要


- 例子
``` 
    CREATE TABLE celebs (id INTEGER, name TEXT, age INTEGER);
```

##创建
```
CREATE TABLE celebs (id INTEGER, name TEXT, age INTEGER);
```

- `CREATE TABLE`分句告诉SQL你要创建一个新表
- `celebs`是新表的名称
- `(id INTEGER, name TEXT, age INTEGER)`是定义表格中的每一列的数据类型的参数表
    - `id` 存储的值为`INTERGER` 类型
    - `name`存储的值为`TEXT`类型
    - `age`存储的值为`INTEGER`
- 这个创建语句结束，此时的数据表相当于只是定义了表头，可以通过插入语句来给数据表增加一行记录

##插入
```
INSERT INTO celebs (id, name, age) VALUES (1, 'Justin Bieber', 21);
```
- `INSERT INTO`语句用于插入一行或者多行记录到数据表中
- `celebs`是待插入一行或多行记录的表格
- `(id, name, age)`用来验证将要插入的每一列的记录的数据类型
- `VALUES`分句声明了后面将要被插入数值,`(1, 'Justin Bieber', 21)`是待插入的记录


##查看整张表
```
SELECT * FROM celebs;
```
