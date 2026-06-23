
适用范围
用于将 Claude Code CLI 接入兼容 Anthropic API 的第三方中转站、代理或网关。

开始前请确认你已获取：

API 密钥 ：进入后台，点击API密钥菜单
API 端点：进入后台，点击API密钥菜单
macOS/Linux/WSL
当前终端临时生效

```
export ANTHROPIC_BASE_URL="你的API 端点"
export ANTHROPIC_AUTH_TOKEN="你的API密钥"
export CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC=1
```

永久生效
将以下内容写入 ~/.zshrc：

```
export ANTHROPIC_BASE_URL="你的API 端点"
export ANTHROPIC_AUTH_TOKEN="你的API密钥"
export CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC=1
```

加载配置：

source ~/.zshrc
如果使用 bash（一般linux或wsl），请改写入 ~/.bash_profile 或 ~/.bashrc。

或者写入配置文件 settings.json
文件路径：

~/.claude/settings.json
示例：
```
{
  "env": {
    "ANTHROPIC_BASE_URL": "你的API 端点",
    "ANTHROPIC_AUTH_TOKEN": "你的API密钥",
    "CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC": "1",
    "CLAUDE_CODE_ATTRIBUTION_HEADER": "0"
  }
}
```
提示
通过环境变量或settings.json配置文件任选其中一种方式即可

Windows
当前终端临时生效

```
$env:ANTHROPIC_BASE_URL="你的API 端点"
$env:ANTHROPIC_AUTH_TOKEN="你的API密钥"
$env:CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC=1
```

永久生效
在windows环境变量中新增系统变量
```
ANTHROPIC_BASE_URL="你的API 端点" 
ANTHROPIC_AUTH_TOKEN="你的API密钥"
CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC=1
```
或者写入配置文件 settings.json
文件路径：

%userprofile%\.claude\settings.json
示例：
```
{
  "env": {
    "ANTHROPIC_BASE_URL": "你的API 端点",
    "ANTHROPIC_AUTH_TOKEN": "你的API密钥",
    "CLAUDE_CODE_DISABLE_NONESSENTIAL_TRAFFIC": "1",
    "CLAUDE_CODE_ATTRIBUTION_HEADER": "0"
  }
}
```
提示
通过环境变量或settings.json配置文件任选其中一种方式即可
