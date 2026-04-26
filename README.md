# xuanhaopin-site-v1

xuanhaopin.com 第一版静态原型。

## 当前内容
- `index.html`：站点首页（V2）
- `trash-bags.html`：家用垃圾袋决策页
- `disposable-gloves.html`：一次性手套决策页骨架
- `storage-bags.html`：保鲜袋决策页骨架
- `assets/`：后续放商品图、站点图标等
- `data/`：后续放商品结构化数据、返佣链接映射

## 当前已完成
- 单页结构：类目规则 + 3 个商品决策块 + FAQ + machine-readable summary
- 已将首页原型替换为京东 3 个真实商品版本（主推 A、一倍；主推 B、京东京造；经济款 C、利得）
- 京东 4 个商品已完成初步抓取整理，拼多多 3 个因登录/壳页问题暂未进入首版
- 已预留 go 链接占位：
  - `/go/trashbag-a-jd`
  - `/go/trashbag-a-tb`
  - `/go/trashbag-a-pdd`
  - `/go/trashbag-b-jd`
  - `/go/trashbag-b-tb`
  - `/go/trashbag-b-pdd`
  - `/go/trashbag-c-jd`
  - `/go/trashbag-c-tb`
  - `/go/trashbag-c-pdd`

## 当前 go 映射
- `go/trashbag-a-jd.html` -> 京东1 -> 一倍抽绳垃圾袋
- `go/trashbag-b-jd.html` -> 京东4 -> 京东京造垃圾袋
- `go/trashbag-c-jd.html` -> 京东2 -> 利得平口垃圾袋

具体映射见：`data/go-links.json`

## 当前已实现
- 本地静态可用的 go 跳转页已经生成到 `go/` 目录
- 页面里的购买按钮已指向本地 go 跳转页

## 下一步需要补的素材
1. 商品图（可选，但建议有）
2. 后续 go 跳转实现
3. 域名部署和日志
4. 拼多多后续如要接入，需要登录态或人工补商品信息
