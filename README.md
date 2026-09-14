# PolyU — Jockey Club Innovation Tower

风格化的香港理工大学赛马会创新楼三维建筑模型。依据多角度照片概括双翼体量、白色曲面飘带、深色玻璃和入口雨棚，不代表测绘尺寸或真实 BIM 数据。

- 拖动旋转，滚轮缩放，右键平移；支持触屏。
- 透视、正视、背面与俯视预设；支持部位选择、自动旋转与夜间光照。
- `app/innovation-tower.ts` 保存程序化模型，`app/page.tsx` 为查看器。

## 本地运行

需要 Node.js 24、pnpm。运行 `pnpm install`，再运行 `pnpm exec vite --config vite.pages.config.ts`。

## 静态构建

运行 `pnpm exec vite build --config vite.pages.config.ts`，输出到 `dist/pages`。仓库子路径通过 `PAGES_BASE_PATH` 设置。

GitHub 线上仓库当前以 main 根目录静态文件发布；源码压缩包 `campus-twin-source.zip` 包含完整工程。解压至独立开发仓库后，可使用 `.github/workflows/pages.yml` 自动构建发布。
