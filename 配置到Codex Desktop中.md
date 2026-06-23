适用范围
用于将 Codex CLI 接入兼容 OpenAI API 的第三方中转站、代理或网关。

开始前请确认你已获取：

API 密钥 ：进入后台，点击API密钥菜单
API 端点：进入后台，点击API密钥菜单
macOS/Linux/WSL
写入配置文件 config.toml
文件路径：

~/.codex/config.toml
~/.codex/auth.json
示例：
```
model_provider = "OpenAI"
model = "gpt-5.4"
review_model = "gpt-5.4"
model_reasoning_effort = "xhigh"
disable_response_storage = true
network_access = "enabled"
windows_wsl_setup_acknowledged = true
model_context_window = 1000000
model_auto_compact_token_limit = 900000

[model_providers.OpenAI]
name = "OpenAI"
base_url = "你的API 端点"
wire_api = "responses"
requires_openai_auth = true
```
```
{
  "OPENAI_API_KEY": "你的API 密钥"
}
```
提示
请确保配置目录存在。macOS/Linux 用户可运行 mkdir -p ~/.codex 创建目录。

Windows
写入配置文件 config.toml
文件路径：
```
%userprofile%\.codex\config.toml
```
```
%userprofile%\.codex\auth.json
```
示例：
```
model_provider = "OpenAI"
model = "gpt-5.4"
review_model = "gpt-5.4"
model_reasoning_effort = "xhigh"
disable_response_storage = true
network_access = "enabled"
windows_wsl_setup_acknowledged = true
model_context_window = 1000000
model_auto_compact_token_limit = 900000

[model_providers.OpenAI]
name = "OpenAI"
base_url = "你的API 端点"
wire_api = "responses"
requires_openai_auth = true
```
```
{
  "OPENAI_API_KEY": "你的API 密钥"
}
```
提示
> 按 Win+R，输入 %userprofile%.codex 打开配置目录。如目录不存在，请先手动创建。
