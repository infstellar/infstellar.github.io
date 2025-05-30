---
title: vscode和ssh设置
date: 2023-04-18 21:17:39
categories: 
- Technology Tools Tips
tags: 
- vscode
- ssh
- clash
---

## ssh rsa-key复制
```powershell
$USER_AT_HOST="";
$PUBKEYPATH="%UserProfile%\.ssh\common_key.pub";
$pubKey=(Get-Content "$PUBKEYPATH" | Out-String);
ssh "$USER_AT_HOST" "mkdir -p ~/.ssh && chmod 700 ~/.ssh && echo '${pubKey}' >> ~/.ssh/authorized_keys && chmod 600 ~/.ssh/authorized_keys"
```

## ssh各种命令

### ssh 重启
- Linux： service sshd restart

### ssh 配置文件路径

/etc/ssh/sshd_config

~/.ssh/authorized_keys