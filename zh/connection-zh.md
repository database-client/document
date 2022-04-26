# 备注

## 缓存

为了提高性能，缓存了数据库信息，如果你的数据库结构在外部发生了变更，需要点击以下按钮刷新缓存。
![](../images/1638342622208.png)

## 先决条件

### SQL Server

如果要通过端口连接到你本机的SQL Server, 通常需要启用TCP/IP连接方式, 详情查看:

[Configure a Server to Listen on a Specific TCP Port - SQL Server | Microsoft Docs](https://docs.microsoft.com/en-us/sql/database-engine/configure-windows/configure-a-server-to-listen-on-a-specific-tcp-port?view=sql-server-ver15#SSMSProcedure)

### SQLite

1. SQLite依靠SQLite外部程序来连接, 如果你的操作系统不是windows, 需要确保你的环境变量中具有sqlite3.
2. 如果你使用sqlite出现错误"unknown command or invalid arguments: "open".", 请考虑降级你的sqlite3版本, 在某些sqlite3版本中.open命令被移除了, 但扩展需要通过open命令才能支持unicode字符.

### MongoDB

MongoDB只有少量的支持, 只建议用于浏览数据.

## 对象筛选

快速筛选数据库对象, VSCode不支持创建输入框, 只能通过这种方式.
![filter](../images/filter.gif)