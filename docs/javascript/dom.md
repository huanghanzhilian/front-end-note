### 访问下一个节点
方法一
``` javascript
function get_nextSibling(n){
    var x=n.nextSibling;
    while (x && x.nodeType!=1){
        x=x.nextSibling;
    }
    return x;
}
```

### 访问元素节点的子节点，返回一个数组
方法一
``` javascript
function get_childNodes(n){
	var addr=[];
	for (var i = 0; i < n.length; i++) {
		if(n[i].nodeType==1){
			addr.push(n[i]);
		}
	}
    return addr;
}
```




