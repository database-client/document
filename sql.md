# SQL

## Execute

In the Database Explorer panel, click the `Open Query` button.

![newquery](images/newquery.jpg)

That will open a SQL editor bind of database, it provider:

1. IntelliSense SQL edit.
2. snippets:`sel、del、ins、upd、joi, selc`...
3. Run selected or current cursor SQL (Shortcut : Ctrl+Enter).
4. Run all SQL (Shortcut : Ctrl+Shift+Enter).

![run](images/run.jpg)

This extension supports codelen, but does not support stored procedures and functions. If you use them frequently, it is recommended to disable codelen

![image](https://user-images.githubusercontent.com/27798227/144196926-e581872e-5392-4744-a646-a644749c548c.png)

## Table Definition

When you move the mouse over the table, the table creation SQL can be displayed, or use the alt+enter shortcut to operate through Code Action (only non-hidden tables can be supported)

![](image/sql/1647176834109.png)
