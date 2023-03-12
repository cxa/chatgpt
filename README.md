# chatgt

ChatGPT in your terminal.

## Installation

Copy `chatgpt` to a directory that is included in `$PATH`, like `/usr/local/bin`. Make sure that:

1. You have `curl` and `jq` installed.
2. You have set the environment variable `export OPENAI_API_KEY="[your key]"`.

## Usage

```sh
chatgpt system_message user_message
```

If only one parameter is passed, it defaults to `user_message`.

`system_message` is used to identify the AI role, like "You are a BASH programming expert," and then ask BASH-related questions. Setting `system_message` is recommended to get more accurate answers.

### Tips

You can alias some commands to use a fixed `system_message`:

```sh
alias bashq='chatgpt "You are a BASH programming expert"'
alias tcn='chatgpt "You are a English-to-Chinese technical document translation expert"'
```
