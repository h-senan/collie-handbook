# 配置文件示例(JSON)
## 项目配置
```json
{
  "name": "公司名<string>",
  "mobilephone": [ "手机号<number>" ],
  "phone": [ "座机号<number>" ],
  "address": "地址<string>",
  "website": "公司网址<string>",
  "aboutTitle": "关于公司标题<string>",
  "aboutContent": "关于公司正文<string>",
  "tabs": [{
    "icon": "tab-icon1<string>",
    "label": "tab标签<string>",
    "pages": [{
      "components": [{
        "type": "组件配型<string>",
        "id": "组件id<string>",
        "data": "组件所需数据<object>"
      }, {
      "type": "组件配型<string>",
      "id": "组件id<string>",
      "data": "组件所需数据<object>"
      }]
    }]
  }, {
    "icon": "tab-icon1<string>",
    "label": "tab标签<string>",
    "pages": [{
      "components": [{
        "type": "组件配型<string>",
        "id": "组件id<string>",
        "data": "组件所需数据<object>"
      }]
    }]
  }]
}
```
## 组件配置
### 轮播组件