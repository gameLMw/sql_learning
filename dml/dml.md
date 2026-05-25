# 数据操作语言（DML）概述

数据库中，数据操作语言（Data Manipulation Language，简称 DML）用于对数据库中的数据进行增、删、改、查等操作。DML 直接作用于数据库表中的记录，是最常见的 SQL 操作类型之一。

## 主要作用

- 插入数据：向表中添加新记录。
- 更新数据：修改已有记录的内容。
- 删除数据：移除不再需要的记录。
- 查询数据：检索和筛选符合条件的数据。

## 常见 DML 命令

- `INSERT`：将新行插入数据库表。
- `UPDATE`：修改表中现有记录的值。
- `DELETE`：删除表中的记录。
- `SELECT`：查询表中的数据。

## 典型使用场景

1. 将用户提交的信息保存到数据库。
2. 更新订单状态或修改客户资料。
3. 删除过期或错误的数据记录。
4. 查询并展示报表、统计结果或数据分析结果。

## DML 与其他 SQL 语言的关系

- DDL（数据定义语言）：用于定义数据库结构，如创建表和索引。
- DML（数据操作语言）：用于对数据本身进行操作。
- DCL（数据控制语言）：用于管理权限和安全。
- TCL（事务控制语言）：用于管理事务的提交和回滚。

## 示例

- 插入数据：
  ```sql
  INSERT INTO employees (id, name, hire_date) VALUES (1, 'Alice', '2026-05-25');
  ```

- 更新数据：
  ```sql
  UPDATE employees SET department = 'Sales' WHERE id = 1;
  ```

- 删除数据：
  ```sql
  DELETE FROM employees WHERE id = 1;
  ```

- 查询数据：
  ```sql
  SELECT id, name, hire_date FROM employees WHERE department = 'Sales';
  ```

## 小结

DML 是日常数据库操作的核心，通过增删改查命令，应用程序可以实现数据的读写和维护，满足业务流程的动态需求。