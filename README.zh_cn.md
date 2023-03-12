# chatgt

终端中的 ChatGPT。

## 安装

复制 `chatgpt` 到 `$PATH` 包含的路径中，比如 `/usr/local/bin`. 请确保：

1. 已安装 `curl` 和 `jq`.
2. 设置环境变量 `export OPENAI_API_KEY="[your key]"`

## 使用方法

```sh
chatgpt system_message user_massage
```

如果只传一个参数，那么默认为 `user_massage`. 

`system_message` 是用来定位 AI 角色的，比如可以设置为「您是一位 BASH 编程专家」，然后提问 BASH 相关的问题。为了得到更精确的答案，建议设置 `system_message`.

### 贴士

你可以 alias 一些命令使用固定的 `system_message`：

```sh
alias bashq='chatgpt "您是一位 BASH 编程专家"'
alias tcn='chatgpt "您是一位中文到英文的技术文档翻译专家"'
```
