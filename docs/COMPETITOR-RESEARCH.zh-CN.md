# 文档扫描竞品调研

**调研日期：** 2026 年 9 月 6 日  
**范围：** 全自动文档照片处理、批量流程、浏览器可用性和扫描效果。  
**证据口径：** 除特别说明外，均采用产品官网或官方帮助文档。

## 结论

自动找边、透视校正和多页扫描已经是行业常见能力。Adobe Scan、CamScanner、Genius Scan、iScanner、Apple 备忘录和 Google Drive 都具备其中多项能力，一些网页扫描工具也支持自动找边和多页 PDF。

[Web Document Scanner](https://web-doc-scanner.app) 的差异化来自一组聚焦的能力组合：

> 面向已有文档照片的浏览器扫描器：批量导入，并默认自动完成找页、拉平和去阴影。

功能列表用于说明各产品具备哪些能力，[同图视觉对比](../benchmark/COMPARISON.zh-CN.md)
则直观展示所选产品处理相同高难度照片时的差异。

## 竞品能力

| 产品 | 已验证优势 | 与本产品相关的差异或限制 | 来源 |
| --- | --- | --- | --- |
| Adobe Scan | 实时找边、自动裁切、图像清理、AI 拉直/曲面校正、导入照片、High-Speed Scan | 必须安装移动 App；扫描保存到 Adobe 云；保留检查和编辑入口 | [Adobe Scan 官方文档](https://www.adobe.com/devnet-docs/adobescan/android/en/scan.html) |
| CamScanner | 批量扫描、自动找边、裁切、透视校正、增强、阴影清理和 OCR | 以 App 为中心；仍提供裁切和滤镜检查流程 | [CamScanner 官方文章](https://blog.camscanner.com/2026/07/24/independent-retailer-month-2026-smarter-document-management-for-small-businesses-with-camscanner/) |
| Genius Scan | 文档检测、背景移除、畸变校正、去阴影、批量扫描 | 必须安装 iOS/Android App；支持端侧处理 | [Google Play 产品页](https://play.google.com/store/apps/details?id=com.thegrizzlylabs.geniusscan.free)、[Genius Scan SDK 功能](https://geniusscansdk.com/features) |
| iScanner | 自动裁切、歪斜/曲面校正、背景清理、多页编辑和 OCR | 扫描依赖 iOS/Android App；产品形态更偏综合文档编辑与管理 | [iScanner 官网](https://iscanner.com/)、[App Store 页面](https://apps.apple.com/us/app/iscanner-pdf-document-scanner/id1040093707) |
| Apple 备忘录 | 自动检测边界并拍摄，可连续添加页面保存成 PDF | 局限于苹果设备，以实时相机拍摄为主 | [Apple iPhone 使用手册](https://support.apple.com/guide/iphone/scan-text-and-documents-iph653f28965/ios) |
| Google Drive | 自动拍摄、裁切旋转、滤镜、清理、多页和可搜索 PDF | 扫描只在移动 App 中提供，网页端没有；文件保存到 Drive | [Google Drive 帮助](https://support.google.com/drive/answer/3145835) |
| Microsoft Lens | 曾经是主要竞品 | 2026 年退役，2026 年 3 月 9 日后不能新建扫描；官方推荐 OneDrive，但 OneDrive 不支持本地保存扫描件 | [微软官方退役通知](https://support.microsoft.com/en-US/lens/retirement-of-microsoft-lens) |
| OnlineCamScanner | 浏览器运行、自动检测四角、多页和 PDF/图片下载 | 官方流程明确包含“调整并裁切”，之后再增强和下载 | [OnlineCamScanner](https://onlinecamscanner.com/) |
| OptiPix Document Scanner | 浏览器本地处理、自动找边、透视校正、多页 PDF | 自动检测不准时仍需手拖四角；核心定位是本地隐私处理 | [OptiPix](https://optipix.art/document-scanner) |

## [Web Document Scanner](https://web-doc-scanner.app) 的产品优势

- 现代浏览器直接使用，不安装扫描 App。
- 可从手机或电脑导入已经拍好的文档照片。
- 单个任务批量处理多张图片（Pro 最多 15 张）。
- 自动找页、拉平、校正和清理。
- 重点处理歪斜、露出桌面和光照不均的照片。
- 导出 PDF、图片或 ZIP。
- 上传图和生成图在 24 小时内自动删除。

## 扫描质量对比

已公开的对比使用同一组原图，重点观察页面几何、背景清理、文字可读性和结果
一致性。综合现有输出，[Web Document Scanner](https://web-doc-scanner.app) 在稳定拉平页面和生成干净、
均匀背景方面表现突出，尤其适合大角度斜拍和光照不均的照片。

实际效果可能随原图、App 版本、设备、滤镜和裁切调整而变化。将每张原图与
全部输出并排公开，使对比过程更透明，也便于直接复核。

## 可复现的扫描效果测试

10 张图片的视觉对比及导出证据保存在
[`../benchmark/COMPARISON.zh-CN.md`](../benchmark/COMPARISON.zh-CN.md)
中。下面的方法说明如何进一步扩展文档类型和拍摄条件。

### 测试集

至少准备 100 张从未用于开发调参的原图：

- 20 张光线均匀的平整打印文档；
- 20 张水平或垂直方向大角度斜拍；
- 20 张带桌面和手部阴影的文档；
- 15 张起皱、折叠或弯曲页面；
- 15 张放在浅色和深色背景上的小票；
- 10 张手写作业。

覆盖多种手机型号、分辨率、纸张颜色、语言和室内光线。每个产品必须使用完全相同、未经修改的原图。

### 参测产品

至少包括：

1. Adobe Scan
2. CamScanner
3. Genius Scan
4. iScanner
5. Apple 备忘录或 Google Drive
6. OnlineCamScanner
7. 另一个以浏览器为主的扫描器
8. [Web Document Scanner](https://web-doc-scanner.app)

使用当时公开版本和默认/自动增强模式。记录版本、日期、平台、套餐和所有非默认设置。

### 客观指标

每页测试：

- **边界准确率：** 自动结果和人工纸张蒙版的交并比。
- **内容保留率：** 保留下来的真实文字/内容区域比例。
- **几何校正：** 文字基线偏离水平以及页面边缘偏离矩形的程度。
- **阴影减少：** 空白纸张区域的亮度方差。
- **可读性：** 所有输出统一使用一个中立 OCR 引擎计算字符错误率。
- **细节保留：** 小字号和细笔画是否完整。
- **人工干预率：** 需要手改四角或滤镜的页面比例。
- **操作成本：** 从导入原图到导出文件的点击数和时间。
- **批次一致性：** 同一文档各页纸张亮度和对比度的差异。

### 盲测

随机打乱并隐藏所有输出的产品名，至少邀请 5 名评审分别评价：

1. 文字可读性；
2. 页面几何是否正确；
3. 背景和阴影是否干净；
4. 外观是否自然；
5. 是否可以直接提交。

评审不能知道每张图来自哪个产品。发布样本数、评分说明、聚合原始分数、置信区间、失败样本和并列结果。

### 如何解读对比结果

对比结论应与测试图片、产品版本和评价维度一起阅读：

- 说明原图来源和处理日期；
- 同时公开原图与处理结果；
- 记录滤镜设置和人工调整；
- 展示表现突出与处理困难的样本；
- 区分视觉观察与 OCR、几何等量化指标。

针对当前测试集，可以将结果概括为：

> “在本次大角度斜拍和光照不均的文档照片测试中，[Web Document Scanner](https://web-doc-scanner.app) 展现出稳定的页面拉平与背景清理效果。”
