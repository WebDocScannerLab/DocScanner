# 拍照转扫描件｜全自动在线文档扫描

**[中文](./README.zh-CN.md)** · **[English](./README.md)**

[Web Document Scanner](https://web-doc-scanner.app/zh/) 是一款**全自动在线文档扫描**工具，可以把手机里已有的文档照片批量变成清晰、拉平的扫描件 PDF。上传一张或多张照片后，系统会自动找页、校正透视、拉平页面、清理阴影并准备导出——不用安装 App，也不用逐页拖动四个裁切点。

<p align="center">
  <a href="https://web-doc-scanner.app/zh/"><img src="https://img.shields.io/badge/立即扫描-打开网页扫描器-2563eb?style=for-the-badge" alt="打开 Web Document Scanner 中文扫描页"></a>
</p>

<p align="center">
  <a href="https://web-doc-scanner.app/zh/">立即扫描</a> ·
  <a href="https://web-doc-scanner.app">English</a> ·
  <a href="https://web-doc-scanner.app/zh/pricing">定价</a> ·
  <a href="https://web-doc-scanner.app/zh/contact">企业 API</a>
</p>

> 这是托管商业产品的公开项目文档，只包含产品介绍，不包含源代码或可私有部署的软件包。

## 为什么选择 Web Document Scanner？

### 从上传到扫描全自动

很多扫描工具围绕实时相机和编辑页面设计。Web Document Scanner 更适合处理已经存在于相册、微信、邮件、隔空投送或共享目录里的照片。添加文件后，处理流程会自动完成：

- 找到纸张并移除背景；
- 校正斜拍造成的透视变形；
- 拉平页面；
- 清理阴影和不均匀光照；
- 增强纸张与文字对比度；
- 整理页面并导出。

需要时仍可旋转和调整顺序，但默认流程不要求逐页拖动四个角。

### 已有照片可批量处理

不必对着相机一页页拍摄、确认和编辑。Pro 单次最多可添加 **15 张图片**。排好顺序后启动一次任务，即可把整批照片处理并导出为 PDF、图片或 ZIP。

这特别适合处理已经从微信、邮件、相册、AirDrop 或共享文件夹收到的文档。

### 专门处理难扫的手机照片

Web Document Scanner 不只是把 JPG 放进 PDF，而是针对手机拍纸张时最影响观感的问题：

- 斜拍造成的梯形和透视变形；
- 深色桌面和多余背景；
- 顶灯形成的阴影与亮斑；
- 灰暗、不均匀的纸张底色；
- 同一批页面之间效果不一致。

质量目标是得到更接近平板扫描仪输出、文字清楚、可以直接提交的页面，而不是一张加了滤镜的裁切照片。

在与 Adobe Scan、CamScanner 和 iScanner 的[同图对比](./benchmark/COMPARISON.zh-CN.md)中，Web Document Scanner 在现有测试结果里展现出稳定的页面拉平、背景清理和批次一致性。所有原图与输出图均已公开，可直接查看对比。

## 和主流扫描工具有什么不同？


| 产品 | 无需安装 App | 导入已有照片 | 自动校正 | 批量 / 多页 | 典型流程 |
| --- | --- | --- | --- | --- | --- |
| **Web Document Scanner** | 是，浏览器运行 | 是 | 找页、拉平、透视和阴影清理 | 是，Pro 单次最多 15 张 | 批量上传 → 自动处理 → 导出 |
| Adobe Scan | 否，移动 App | 是 | 自动裁边、清理和 AI 拉直 | 是，High-Speed Scan | 拍摄/导入 → 检查编辑 → 保存到 Adobe 云 |
| CamScanner | 否，移动 App | 是 | 自动裁边、透视校正和增强 | 是 | 拍摄/导入 → 检查裁切/滤镜 → 导出 |
| iScanner | 否，移动 App | 是 | 自动裁切、畸变校正和清理 | 是 | 拍摄/导入 → 修饰编辑 → 导出 |

扫描市场已经有很多成熟产品。Web Document Scanner 的定位是以下能力的组合：

1. **手机和电脑都能直接打开浏览器使用。**
2. **批量导入已经拍好的照片**，不局限于现场逐页拍摄。
3. **自动处理是主流程**，不是先进入四角裁切编辑器。
4. **针对歪斜与重阴影照片做拉平和清理。**
5. **直接导出 PDF、图片或 ZIP。**

## 怎样在线扫描文档？

1. **上传一张或多张照片。** 选择设备里已有的 JPG 或 PNG。
2. **整理页面。** 需要时调整顺序或旋转。
3. **开始扫描。** 自动运行找页、拉平和清理。
4. **导出结果。** 下载 PDF、单页图片或 ZIP。

免费版每天可扫描 **1 张图片**，结果带水印。[Pro](https://web-doc-scanner.app/zh/pricing) 不限每天次数、没有水印，单个任务最多处理 **15 张图片**。

## 扫描效果好，具体指什么？

扫描质量应该用统一测试衡量，而不是只写一句绝对化口号。对本产品来说，“效果更好”包括：

- 自动找页后保留更多真实纸张内容；
- 页面几何和文字行更端正；
- 桌面背景和阴影更少；
- 文字更清晰，同时不过度压黑细笔画；
- 同一批页面的白平衡和对比度更一致；
- 需要人工修正的页面更少；
- 从导入到可用文件所需操作更少。

[已经公开的同图对比](./benchmark/COMPARISON.zh-CN.md)显示，在大角度斜拍和
光照不均的文档照片中，Web Document Scanner 的页面几何、背景清洁度和输出
一致性表现突出：

> **把难处理的手机文档照片变成更干净、更平整的扫描件：浏览器中批量上传，全自动处理。**

## 常见使用场景

- [作业照片合成一份 PDF](https://web-doc-scanner.app/zh/scan-homework)
- [发票和收据报销扫描](https://web-doc-scanner.app/zh/scan-receipt)
- [把照片做成扫描件](https://web-doc-scanner.app/zh/photo-to-scanned-document)
- [JPG、PNG 转扫描件 PDF](https://web-doc-scanner.app/zh/image-to-scanned-pdf)
- [在线图片扫描](https://web-doc-scanner.app/zh/online-image-scanner)
- 企业文档扫描 API

## 产品能力

- 全自动找页和增强
- 批量上传、排序和旋转
- 透视校正与页面拉平
- 阴影和不均匀背景清理
- PDF、图片和 ZIP 导出
- 英文与简体中文界面
- Google 登录
- 企业 API
- 上传图和生成图在 24 小时内自动删除

当前产品输出扫描图和 PDF，不提供 OCR 或表格金额提取。

## 隐私

上传的照片和生成的扫描件会在 **24 小时内自动删除**。我们不出售上传的文档，也不会把它们用于广告。支付由 Stripe 处理，登录使用 Google OAuth。

详见[隐私政策](https://web-doc-scanner.app/zh/privacy-policy)和[服务条款](https://web-doc-scanner.app/zh/terms-of-service)。

## 常见问题

### 需要安装 App 吗？

不需要。用手机或电脑的现代浏览器打开 [web-doc-scanner.app](https://web-doc-scanner.app/zh/) 即可。

### 需要手动拖四个角吗？

不需要。默认流程会自动找页和校正。必要时仍可旋转和调整页面顺序。

### 可以一次上传多张照片吗？

可以。Pro 单个扫描任务最多支持 15 张。添加照片、排好顺序，再统一处理。

### 和图片转 PDF 一样吗？

不一样。普通转换器只是把原照片放进 PDF。Web Document Scanner 会先检测并拉平页面，再清理图像。

### 效果一定比所有扫描 App 好吗？

实际结果会受到纸张形状、光线、相机质量、模糊和遮挡影响。在已公开的测试集中，Web Document Scanner 在自动拉平、背景清理和复杂斜拍照片的一致性方面表现突出。可以直接查看[同图对比结果](./benchmark/COMPARISON.zh-CN.md)。

### 提供 API 吗？

提供。[联系我们](https://web-doc-scanner.app/zh/contact)获取企业 API 用量、速率、支持和发票结算方案。

## 开始扫描

[打开中文扫描页 →](https://web-doc-scanner.app/zh/)

[Scan document photos online →](https://web-doc-scanner.app)

---

**Web Document Scanner** · [web-doc-scanner.app](https://web-doc-scanner.app) 
