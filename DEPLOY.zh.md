# Evidentia 应用包

这个文件夹就是完整的 Evidentia 应用，可以直接部署成网站，再安装到电脑或手机上。

## 文件说明

| 文件 | 作用 |
|---|---|
| `index.html` | 整个网站和工作台（7 种语言） |
| `manifest.webmanifest` | 应用信息：名称、图标、独立窗口打开 |
| `sw.js` | 离线支持：打开过一次后，断网也能使用 |
| `icons/` | 应用图标 |

## 第 1 步：部署到网上（任选一种，都免费）

安装功能需要 https 网址，直接双击 `index.html` 打开时不能安装。

**Netlify Drop（最简单）**
1. 打开 https://app.netlify.com/drop
2. 把整个 `Evidentia-App` 文件夹拖进去
3. 登录后得到网址，可以在设置里改成 `evidentia-xxx.netlify.app`

**Cloudflare Pages**
1. 登录 Cloudflare → Workers & Pages → Create → Pages → Upload assets
2. 上传这个文件夹，项目名填 `evidentia`
3. 得到 `evidentia.pages.dev` 这样的网址

**GitHub Pages（适合放进作品集）**
1. 新建一个仓库，上传这个文件夹里的所有文件
2. Settings → Pages → Branch 选 `main`，保存
3. 得到 `你的用户名.github.io/仓库名`

## 第 2 步：安装成应用

- **Mac / Windows（Chrome 或 Edge）**：打开网址，点地址栏右侧的“安装”图标。
- **Mac（Safari）**：菜单栏 文件 → 添加到程序坞。
- **iPhone / iPad（Safari）**：分享 → 添加到主屏幕。
- **Android（Chrome）**：菜单 → 安装应用。

安装后它会有自己的图标，在独立窗口中打开，直接进入工作台。

## 数据说明

- 项目数据保存在当前浏览器、当前网址下，不会上传到服务器。
- 换网址、换浏览器或换设备时，数据不会自动带过去。可以在工作台右上角 ••• 菜单中“导出项目 (.json)”，再到新地方“导入项目”。
- 在 Claude 预览链接里建的项目，也用同样的方法导出、导入过来。

## 以后更新

修改 `index.html` 后，把 `sw.js` 第一行的版本号改一下（例如 `evidentia-v2`），重新上传。已安装的用户下次打开就会拿到新版本。
