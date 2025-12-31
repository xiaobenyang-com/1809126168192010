# 查现代汉语词典 Lookup Modern Chinese Dictionary

从现代汉语词典中检索单词释义，为用户提供便捷的词典查询服务。
Search for word definitions from modern Chinese dictionaries to provide users with convenient dictionary query services.## 工具列表 Tool List

本MCP服务封装下列工具，可让模型通过标准化接口调用以下功能。 本MCP服务封装下列工具，可让模型通过标准化接口调用以下功能。

| 工具 Tool   | 描述 Description         |
|-------|--------------------|
| lookup_word | 查单词 |


## 检查服务 ## Inspector

工具在线测试： [https://mcp.xiaobenyang.com/inspector/1809126168192010](https://mcp.xiaobenyang.com/inspector/1809126168192010)

Online Tool test [https://mcp.xiaobenyang.com/inspector/1809126168192010](https://mcp.xiaobenyang.com/inspector/1809126168192010)

## 服务配置 MCP Server Config


> #### 如何获取 XBY-APIKEY ？ How to get XBY-APIKEY ?
> 访问小笨羊科技网站 [https://xiaobenyang.com](https://xiaobenyang.com)，注册用户即可获得APIKEY
> Visit XiaoBenYang website [https://xiaobenyang.com](https://xiaobenyang.com), register and get the APIKEY.

### SSE
```json
{
  "mcpServers": {
    "查现代汉语词典": {
      "headers": {
        "XBY-APIKEY": "<YOUR_XBY_APIKEY>"
      },
      "type": "sse",
      "url": "https://mcp.xiaobenyang.com/1809126168192010/sse"
    }
  }
}
```
### STREAMABLE HTTP
```json
{
  "mcpServers": {
    "查现代汉语词典": {
      "headers": {
        "XBY-APIKEY": "<YOUR_XBY_APIKEY>"
      },
      "type": "streamable_http",
      "url": "https://mcp.xiaobenyang.com/1809126168192010/mcp"
    }
  }
}
```
### STDIO
```json
{
    "mcpServers": {
        "查现代汉语词典": {
          "command": "npx",
          "args": [
            "-y",
            "xiaobenyang-mcp"
          ],
          "env": {
            "XBY_APIKEY": "<YOUR_XBY_APIKEY>",
            "mcpId": "1809126168192010",
          },
          "transport": "stdio"
        }
      }
}

```
