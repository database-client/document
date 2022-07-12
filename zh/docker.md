### Docker

**什么时候你需要这个扩展**?

尽管微软提供了Docker的扩展程序, 但只能连接到本机的docker, 当你需要管理多台服务器上的Docker时, 它无能为力, 这个时候这个扩展可以帮助你做到.

**使用步骤**:

Docker提供了HTTP管理接口, 默认情况下是禁用的, 你需要手动操作开启它.

1. 编辑Docker服务: `vim /usr/lib/systemd/system/docker.service`, Find ExecStart, add `-H tcp://127.0.0.1:2375 --tls=false` at the end of the line
2. 重启Docker: `systemctl daemon-reload && systemctl restart docker`

对于远程的docker, 你应该始终通过ssh隧道连接来保证安全.

![1657606532705](../image/connection/1657606532705.png)
