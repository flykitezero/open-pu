# 贡献指南

感谢你对乐谱编排器项目的关注！我们欢迎各种形式的贡献。

## 如何贡献

### 报告 Bug

如果你发现了 Bug，请通过 [Issue](https://github.com/yourusername/score-arranger/issues) 报告，并包含以下信息：

- 问题的简要描述
- 复现步骤
- 期望行为 vs 实际行为
- 浏览器版本和操作系统
- 截图（如有）

### 提交新功能建议

有新功能的想法？欢迎提交 Issue 讨论：

- 清晰地描述功能
- 解释为什么这个功能有用
- 提供可能的使用场景

### 提交代码

1. **Fork 项目**
   ```bash
   git clone https://github.com/yourusername/score-arranger.git
   cd score-arranger
   ```

2. **创建分支**
   ```bash
   git checkout -b feature/your-feature-name
   # 或
   git checkout -b fix/bug-description
   ```

3. **编写代码**
   - 遵循现有的代码风格
   - 添加必要的注释
   - 确保代码能在主流浏览器运行

4. **提交修改**
   ```bash
   git add .
   git commit -m "feat: 添加新功能描述"
   ```

   提交信息格式：
   - `feat:` 新功能
   - `fix:` 修复 Bug
   - `docs:` 文档更新
   - `style:` 代码格式（不影响功能）
   - `refactor:` 代码重构
   - `perf:` 性能优化
   - `test:` 测试相关
   - `chore:` 构建过程或辅助工具的变动

5. **推送并创建 Pull Request**
   ```bash
   git push origin feature/your-feature-name
   ```

## 代码规范

### HTML

- 使用语义化标签
- 保持缩进一致（2 个空格）
- 属性使用双引号

### CSS

- 使用 CSS Variables 管理主题色
- 类名使用小写和连字符（kebab-case）
- 避免过深的选择器嵌套

### JavaScript

- 使用 ES6+ 语法
- 变量使用 `const` 或 `let`，避免 `var`
- 函数使用箭头函数（适当场景）
- 添加必要的注释

## 开发环境

本项目是纯前端项目，无需构建工具：

```bash
# 方式一：直接打开
open index.html

# 方式二：本地服务器
python -m http.server 8080
# 访问 http://localhost:8080
```

## 测试

在提交前，请确保：

- [ ] 功能在 Chrome、Firefox、Safari 最新版测试通过
- [ ] 深色/浅色主题切换正常
- [ ] 导出功能（PDF/PNG/JSON）正常工作
- [ ] 移动端基本可用

## 行为准则

- 尊重所有参与者
- 接受建设性的批评
- 关注对社区最有利的事情

## 需要帮助？

如有任何问题，欢迎：

- 提交 [Issue](https://github.com/yourusername/score-arranger/issues)
- 发送邮件到 your.email@example.com

再次感谢你的贡献！
