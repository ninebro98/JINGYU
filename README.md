# JINGYU Christmas Tree (V9.1 Ultra Stable)

这是一个基于 Three.js + Bloom 后期处理 + MediaPipe Hands 的互动圣诞树页面。

## 运行方式
- GitHub Pages 直接访问即可（HTTPS 环境支持摄像头）
- 若摄像头权限拒绝或设备不支持：点击页面可切换“点亮/熄灭”（用于演示）

## 常见问题
### 页面黑屏/空白
- 确保脚本依赖顺序正确，尤其是 Three.js 后期处理需要 `Pass.js`
- 本项目 index.html 已包含 Pass.js，并有错误浮层提示

### 摄像头无法使用
- 需要 HTTPS 或 localhost
- 浏览器需允许摄像头权限

## 可选：把依赖本地化（不走 CDN）
如果你想把 three.js / postprocessing 都放进仓库本地，建议目录：
/vendor/three.min.js
/vendor/Pass.js
/vendor/EffectComposer.js
/vendor/RenderPass.js
/vendor/UnrealBloomPass.js

然后把 index.html 里对应 script 的 src 改成 /vendor/xxx.js
