# api

|method |api   |desc   |
| ------------ | ------------ | ------------ |
|POST   |api.aminer.cn/api/bifrost/person/:id/hide   |隐藏一个专家，在profile和search页面是看不到   |
|DELETE   |api.aminer.cn/api/bifrost/person/:id/hide   |隐藏的专家可见   |
|POST |platform.permission.SetSystemFunctionPermissions |给系统设计权限 |
|POST |platform.permission.GetSystem | 查看系统下有所有的权限 system:[] |

## Chenjing Bai 数据修改的api
|  method | api  |exp | desc  |
| ------------ | ------------ | ------------ | ------------ |
|GET   | innova.aminer.cn/get/inst/personlist   |innova.aminer.cn/get/inst/personlist?url=http://www.cs.tsinghua.edu.cn/publish/cs/4797/index.html   |根据单位的教师名录url，返回名单，包括姓名和主页地址|
|POST   | innova.aminer.cn/save/inst/personlist   | ```json
{
     "staff":[{
        "name": "张三",
        "url":  "http://www.cs.tsinghua.edu.cn/publish/cs/4616/2010/20101224151607905825086/20101224151607905825086_.html",
        "org":"清华大学"
    }],
    "creator":"Test Test",
    "creator_id":"5b3d921b530c70c094471a58"
   }

```  |将机构抓下的名单保存为抓取任务|
