# Jiguan-Panel
Jiguan-Panel极光面板docker镜像
# 推送镜像
- 登录 GitHub Container Registry： 在终端或命令行中，使用 GitHub 用户名和 GitHub 的个人访问令牌（PAT）登录 GitHub Container Registry。
```bash
echo <PAT> | docker login ghcr.io -u <your-github-username> --password-stdin
```
```bash
- 将 <PAT> 替换为个人访问令牌，将 <your-github-username> 替换为 GitHub 用户名。
- 如：echo ghp_lgwY7MPK3lLLlJfP8hRApQ***** | docker login ghcr.io -u dogwalkerg --password-stdin
```
