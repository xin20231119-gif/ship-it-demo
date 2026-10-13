# Ship It · 第一个上线 Demo

最小可上线的静态页面，对应「全栈交付上线」目标的第一个里程碑。

## 本地预览

直接用浏览器打开 `index.html` 即可。

## 上线步骤

1. 在 GitHub 新建仓库（比如 `ship-it-demo`），不要勾选初始化 README/许可证
2. 在本目录依次执行（注意先统一分支名为 main，避免与 GitHub 默认分支不一致）：

   ```bash
   git init -b main
   git add .
   git commit -m "ship it: first deployable demo"
   git remote add origin https://github.com/<你的用户名>/ship-it-demo.git
   git push -u origin main
   ```

3. 打开 Vercel → Add New Project → Import 刚才的仓库 → Deploy
4. 拿到 `https://xxx.vercel.app` 线上地址，浏览器打开验证

> 排错：如果打开线上地址跳出 Vercel 登录页，去项目 **Settings → Deployment Protection** 把生产环境保护关掉后 Redeploy。生产域名默认是公开的，一般不需要动。

## 验收标准

- 线上地址可公开访问
- 页面上的「上线检查清单」5 项全部勾选
