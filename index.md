# SQL語法

每次要用SQL語法時都還要查老半天，應該是下次要用SQL時已經不知道過了幾百年了，所以把常用的語法整理到這頁要找比較方便

## SQL簡介

SQL是結構化查詢語言Structured Query Language的縮寫

[維基百科](https://zh.wikipedia.org/zh-tw/SQL)


資料庫(Database)：是組織和儲存資料的集合。可以包含一個以上的表

## 常用指令

### 建立資料表

```sql
CREATE TABLE ExampleTable (_AI INTEGER PRIMARY KEY AUTOINCREMENT,Topic TEXT,Message TEXT);
```

可以加上IF NOT EXISTS來判斷資料表是否存在，不存在才建立

```sql
CREATE TABLE IF NOT EXISTS ExampleTable (_AI INTEGER PRIMARY KEY AUTOINCREMENT,Topic TEXT,Message TEXT);
```

上述指令會建立一個新的資料表（不存在才建立）

資料表名稱為ExampleTable

表中有3個欄位

- _AI：是一個Integer型態的主鍵，並套用AUTOINCREMENT屬性，表示在插入新資料時此欄位會自動遞增
- Topic：是一個TEXT型態的欄位，可以儲存字串資料
- Message：是一個TEXT型態的欄位，可以儲存字串資料

執行結果
![Image](./images/建立資料表.png)