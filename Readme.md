## jQuery中的Ajax

### 复习Ajax怎么用jQuery来实现

```javascript
$.ajax("b.json",{
    //请求的类型
    "type" : "get",
    "data" : {
        "name": "xiaohong"
        "age" : "18"
    }
    //成功后做的事
    "success": function(data){
        alert(type of data);

    },
    //错误做的事情
    "error" : function(XMLHttpRequest,textStatus, errprThrown){
        alert(errorThrown);
    }
})


```# ajax_injQuery
