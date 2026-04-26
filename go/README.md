# go 链接层

当前首版映射：

- `/go/trashbag-a-jd` -> 京东1 -> 一倍抽绳垃圾袋 8卷120只 加厚大号手提厨房家用款
- `/go/trashbag-b-jd` -> 京东4 -> 京东京造 背心式垃圾袋 45×60cm 300只 8μ 中号加厚款
- `/go/trashbag-c-jd` -> 京东2 -> 利得平口垃圾袋 45×50cm 600只 家用办公经济款

当前还未实现真正跳转逻辑，现阶段先把映射关系固定在 `data/go-links.json` 中。

后续部署时可用：
- Vercel Functions
- Cloudflare Workers
- Netlify Functions

实现按路径读取 key，再 302/307 跳转到对应返佣链接。
