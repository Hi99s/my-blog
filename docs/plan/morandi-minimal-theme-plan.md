# 莫兰迪极简主题计划

## Overview

将站点从高饱和可爱风格调整为极简莫兰迪色系，去除页脚，统一中文文案，并保持博客文章模板简洁、安静、适合阅读。

## Current Problem Analysis

上一版视觉包含较多动画、蓝色装饰和英文展示文案，不符合当前“极简、莫兰迪、中文博客”的方向。页面还存在 Astro 模板示例文章中的英文标题、摘要和正文，需要一并清理。

## Strategy and Approach

使用低饱和米色、灰绿、陶土和雾灰建立主题。全站保留头部导航，删除页脚组件和页面引用。首页、文章列表、文章详情和关于页统一使用中文文案。

## Implementation Steps

- ✅ 扫描 Footer 引用和英文展示文案
- ✅ 重写全局莫兰迪主题样式
- ✅ 重构 Header 和 HeaderLink
- ✅ 删除 Footer 组件并移除页面引用
- ✅ 重构首页、文章列表和文章模板
- ✅ 中文化关于页和示例文章内容
- ✅ 运行构建验证

## Timeline

计划在当前工作回合内完成调整和构建验证。

## Risk Assessment

主要风险是删除页脚后仍有残留引用、Tailwind 类名写错导致构建失败、示例文章残留英文展示文本。通过全文搜索和构建验证降低风险。

## Success Criteria

- 全站采用极简莫兰迪色系
- 页面不再渲染 Footer
- 导航、首页、文章列表、文章详情、关于页展示文案为中文
- `npm run build` 成功

## Progress Tracking

- ✅ 主题方向已切换
- ✅ 组件和页面已调整
- ✅ 示例内容已中文化
- ✅ 构建验证完成

## Related Files

- `src/styles/global.css`
- `src/components/BaseHead.astro`
- `src/components/Header.astro`
- `src/components/HeaderLink.astro`
- `src/components/FormattedDate.astro`
- `src/pages/index.astro`
- `src/pages/blog/index.astro`
- `src/pages/about.astro`
- `src/layouts/BlogPost.astro`
- `src/content/blog/`
- `src/consts.ts`
