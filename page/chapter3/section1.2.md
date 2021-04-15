# 配置文件
可以为书籍增加各种配置，配置文件名为book.json,内容为json格式

## 基本配置
### title
  
  书名，默认从README.md文件中提取

### description

  描述，默认从README.md文件中提取

### author

  作者名

### isbn
  
  国际标准书号 ISBN 

### language
  
  本书的语言类型, [ISCODE](https://en.wikipedia.org/wiki/List_of_ISO_639-1_codes)
  默认en,简体中文为zh-hans
  
### gitbook
  
  声明使用的版本号

### structure
结构配置，可以指定readme和summary文件
不使用默认的readme、summary

```
{
    "structure": {
        "readme": "intro.md",
        "summary": "contents.md",
    }
}
```
### links
  
  links可以用来增加sidebar和分享链接按钮
  
  ```
    "links": {
      "sidebar": {
        "微店": "https://www.weidian.com"
      },
      "sharing": {
        "google": null,
        "facebook": null,
        "twitter": null,
        "weibo": "https://www.weibo.com",
        "all": null
      }
    }
  ```
  
  
