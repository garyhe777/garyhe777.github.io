# Linux / Git 命令

## Linux 常用命令

### 文件与目录

| 命令 | 说明 |
|---|---|
| `ls -la` | 列出所有文件（含隐藏），显示详情 |
| `cd / pwd` | 切换目录 / 显示当前路径 |
| `cp / mv / rm` | 复制 / 移动 / 删除 |
| `find . -name "*.log"` | 递归搜索文件 |
| `grep -rn "keyword" .` | 递归搜索内容 |

### 权限管理

- `chmod 755 file`：设置文件权限（rwxr-xr-x）
- `chown user:group file`：修改所有者
- `sudo`：以超级用户权限执行命令

### 进程与网络排查

| 命令 | 说明 |
|---|---|
| `ps aux` | 查看所有进程 |
| `top / htop` | 实时进程监控 |
| `kill -9 <pid>` | 强制终止进程 |
| `netstat -antp` | 查看网络连接与端口 |
| `ss -tulnp` | 查看监听端口 |
| `curl / wget` | 发起 HTTP 请求 / 下载文件 |

---

## Git 基础

```bash
git clone <url>        # 克隆仓库
git add .              # 暂存所有改动
git commit -m "msg"    # 提交
git log --oneline      # 简洁查看历史
git diff               # 查看未暂存改动
```

## Git 协作

```bash
git branch feature     # 新建分支
git checkout feature   # 切换分支
git merge feature      # 合并分支到当前
git rebase main        # 变基到 main
git stash              # 临时保存工作区
git stash pop          # 恢复最近 stash
```

## Git 排错

```bash
git reflog             # 查看所有操作历史（找回误删提交）
git reset --hard HEAD~1  # 回退到上一个提交（危险：丢失改动）
git reset --soft HEAD~1  # 回退提交，保留改动到暂存区
git cherry-pick <sha>  # 将指定提交应用到当前分支
git revert <sha>       # 创建一个反向提交（安全撤销）
```
