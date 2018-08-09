## ajax

```
var request;
if(window.XMLHttpRequest){
    request = new XMLHttpRequest(); //IE7+、Firefox、Chrome、Opera、Safari  
}else{
    request = new ActiveXObject("Microsoft.XMLHTTP"); //IE6、IE5
}
request.open("POST","get.php",true);
request.send();
request.onreadystatechange = function(){
    if(request.readyState===4 && request.status===200){
        //做一些事情 request.responseText
    }
}
```

