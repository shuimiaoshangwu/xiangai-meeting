# 会议回放页（扫码跳转网页）

手机扫二维码 → 打开本页面 → 显示会议直播黑框 + "该会议已结束" + 会议名称/时间 + 参会人数。

## 文件说明

- `index.html` —— 页面本体，所有会议信息都在里面（搜索【占位】逐项替换）
- `images/bg.jpg` —— 背景图，**换成自己的图片：直接替换这个文件，文件名保持 bg.jpg 不变**

## 部署到 GitHub Pages（5 分钟，全网页操作，无需命令行）

1. 打开 https://github.com/new ，登录你的 GitHub 账号
   - Repository name 随便取（比如 `meeting-page`），选择 **Public**
   - 点 **Create repository**
2. 在新仓库页面点 **uploading an existing file**（上传已有文件链接）
   - 把 `index.html` 拖进去，再拖 `images` 文件夹（或先在 `images` 里选 bg.jpg，网页上传时输入路径 `images/bg.jpg`）
   - 点 **Commit changes** 提交
3. 进入仓库 **Settings → Pages**（设置 → Pages）
   - Source 选 **Deploy from a branch**，Branch 选 `main`、目录 `/ (root)`
   - 点 **Save**，等 1~2 分钟
4. 页面顶部会显示你的公共网址，格式为：
   ```
   https://你的用户名.github.io/meeting-page/
   ```
   这就是最终二维码指向的网址。

## 生成二维码

把上面的 github.io 网址发给我，我帮你生成二维码图片；或自己用任何二维码工具（如草料二维码 https://cli.im ）输入网址即可生成。

## 后续修改

改了 `index.html` 或换了背景图后，重新上传文件到同一仓库覆盖即可，网址和二维码都不用变。
