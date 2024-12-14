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
- Login Succeeded   #登陆成功
- 退出登陆：
- docker logout ghcr.io    #退出登陆-正在删除ghcr.io的登录凭据
# 修改本地镜像名称为github对应名称才可以上传Github仓库
- 产看本地镜像：
  ```bash
     docker images
  ```
  - 修改本地镜像名称：
    ```bash
    docker tag 镜像名或镜像ID
    ```
    - 推送镜像到gitHub仓库：
    - 首先GitHub仓库新建一个仓库名称，名称不能大写，不能特殊符号否则上传推送不了！
    ```bash
       docker push ghcr.io/dogwalkerg/jiguanpanel/jiguanpanel-frontend
    ```
