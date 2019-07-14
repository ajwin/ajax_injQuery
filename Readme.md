# ajax_injQuery
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
```
```JS
//JS ajax模板再次复习一下啊
var xhr = new XMLHttpRequest();	//不兼容，能力检测

xhr.onreadystatechange = function(){
	if(xhr.readyState == 4){
		if(xhr.status >= 200 && xhr.status < 300 || xhr.status == 304){
			//正面的HTTP状态码
			alert(xhr.responseText);
}
xhr.open("post","check.php",true);


//ie中的Ajax兼容问题，进行能力检测

if(window.XMLHttpRequest){
				var xhr = new XMLHttpRequest();
}else{
    var xhr = new ActiveXObject("Microsoft.XMLHTTP");
}

```

