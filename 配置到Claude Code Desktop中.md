适用范围
用于将 Claude Desktop 接入兼容 Anthropic API 的第三方中转站、代理或网关。

提示
Claude Desktop 需要在V1.3883.0及之后的新版本

开始前请确认你已获取：

API 密钥 ：进入后台，点击API密钥菜单
API 端点：进入后台，点击API密钥菜单
步骤1：打开 Claude Desktop 并启用开发者模式
打开 Claude Desktop，先不要登录官方账号。
如果当前界面不好直接点菜单，可以按键盘 Tab 切到左上角菜单区域，再按回车打开菜单。
在顶部菜单栏选择 Help（帮助） → Troubleshooting（疑难解答）。
在弹出的子菜单里点击 Enable Developer Mode（启用开发者模式）。
<img width="599" height="500" alt="image" src="https://github.com/user-attachments/assets/67e65fec-54d9-401f-94cb-8de66d442f26" />


步骤 2：进入第三方 API 配置页面
点击新出现的 Developer 菜单。
选择 Configure Third-Party Inference…（配置第三方推理…）。
<img width="513" height="500" alt="image" src="https://github.com/user-attachments/assets/7348b9ef-256a-40dd-a198-b017b351dba9" />

步骤 3：填写 Base URL 和 API Key
<img width="1800" height="1440" alt="image" src="https://github.com/user-attachments/assets/326d0323-6856-4a2d-948a-34b122fe398c" />


步骤 4：验证是否成功
配置完成后，Claude Desktop 可能会提示重启；如果没有提示，也建议手动完全退出后重新打开。
重新打开后，进入 Cowork、Code 或 Projects 相关页面。
输入一个简单问题测试。
如果模型能正常响应，或者界面中显示的是你第三方 API 提供的模型，就说明配置成功。
<img width="3600" height="2142" alt="image" src="https://github.com/user-attachments/assets/3c01a68b-9930-42a7-b167-22ddc44d09d9" />
