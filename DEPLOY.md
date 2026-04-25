# xuanhaopin 部署说明（最短版）

## 当前 deploy 目录内容

- `index.html`
- `site-index.html`
- `data.json`
- `robots.txt`
- `sitemap.xml`
- `assets/`
- `photo/`
- `go/`

这是当前可直接用于静态部署的版本。

---

## 推荐上线方式

### 方案
- GitHub 仓库
- Vercel 部署
- 绑定域名 `xuanhaopin.com`

---

## 最短步骤

### 1. 新建 GitHub 仓库
例如：
- `xuanhaopin-site`

### 2. 把当前 deploy 目录内容作为仓库根目录上传
建议上传的是 `deploy/` 里面的文件本身，不是把 `deploy` 作为多一层子目录。

也就是仓库根目录应该直接看到：
- `index.html`
- `assets/`
- `photo/`
- `go/`

### 3. 注册并登录 Vercel
导入你的 GitHub 仓库。

### 4. 部署
因为这是纯静态页：
- Framework Preset 可选 Other
- 不需要复杂构建命令
- Output Directory 留空即可

### 5. 绑定域名
在 Vercel 项目里添加：
- `xuanhaopin.com`
- 如果需要，也可加 `www.xuanhaopin.com`

### 6. 在域名服务商处配 DNS
按 Vercel 提示配置解析记录。

---

## 当前 go 跳转实现方式

当前 `go/` 目录下是静态 HTML 跳转页：
- `go/trashbag-a-jd.html`
- `go/trashbag-b-jd.html`
- `go/trashbag-c-jd.html`

第一版可以先这样上线。

后续如果要：
- 统计点击
- 动态换链接
- 做更稳的中转

再升级为：
- Vercel Functions
- Cloudflare Workers

---

## 上线前建议再检查

1. 页面在浏览器里是否正常显示
2. 三个商品图是否都能打开
3. 三个 go 链接是否都能跳京东
4. 域名绑定后再看一次移动端显示
