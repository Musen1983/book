# 常用插件

gitbook默认提供了一些插件如导航栏搜索、代码高亮、分享、字体设置、热加载

除了这些之外，还可以在配置文件中配置安装,如图形、侧边栏调节、回到顶部、代码拷贝等

### 配置插件

首先需要在配置文件中，添加插件名，插件配置中，增加配置

配置完成后，运行gitbook install 安装插件

#### 主题
默认主题是黑白的，theme-comscore插件可以让各级标题拥有不同的颜色
```
  "plugins": [
    "theme-comscore"
  ]
```
#### 信息框
> [!NOTE]
> 漂亮的引用

#### 页脚插件
```
  "plugins": [
    "tbfed-pagefooter"
  ],
  "plunginsConfig": {
    "tbfed-pagefooter": {
      "modify_label": "该文件修订时间：",
      "modify_format": "YYYY-MM-DD HH:mm:ss"
    }
  }
```

![footer](../../images/footer.png)

#### 侧边栏可调节
```
"plugins": [
    "splitter"
  ]
```
#### 代码拷贝
```
  "plugins": [
    "code"
  ]
  "plunginsConfig": {
    "code": {
      "copyButtons": true
    }
  }
```
#### 回到顶部
```
  "plugins": [
    "back-to-top-button"
  ]
```

#### Chart图形
{% chart %}
{
    "data": {
        "type": "bar",
        "columns": [
            ["data1", 30, 200, 100, 400, 150, 250],
            ["data2", 50, 20, 10, 40, 15, 25]
        ],
        "axes": {
            "data2": "y2"
        }
    },
    "axis": {
        "y2": {
            "show": true
        }
    }
}
{% endchart %}


#### 其他
可以去npm上搜索gitbook-plugin [plugin](https://www.npmjs.com/search?q=gitbook-plugin)


