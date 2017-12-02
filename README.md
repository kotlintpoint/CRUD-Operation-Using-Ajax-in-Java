# CRUD-Operation-Using-Ajax-in-Java

###### AJAX = Asynchronous JavaScript and XML.

- AJAX is about loading data in the background and display it on the webpage, without reloading the whole page.
- Applications using AJAX: Gmail, Google Maps, Youtube, and Facebook tabs.
- jQuery provides several methods for AJAX functionality
- With the jQuery AJAX methods, you can request text, HTML, XML, or JSON from a remote server using both HTTP Get and HTTP Post

## Without JQuery
```
var xhttp = new XMLHttpRequest();                //Create an XMLHttpRequest Object


xhttp.onreadystatechange = function() {
  if (this.readyState == 4 && this.status == 200) {
    document.getElementById("demo").innerHTML = this.responseText;
  }
};

xhttp.open("GET", "ajax_info.txt", true);        //open(method, url, async)
xhttp.send();                                    //Sends the request to the server  (used for GET)
//	xhttp.send(string)                           Sends the request to the server (used for POST)

```

## With Jquery

```
<script type="text/javascript" src="//ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.min.js"></script>

function f1(){
$.ajax({
		type : "post/get",
		url : "url/servlet",
		data : "data",
		success : function(msg) {
			alert(msg)
		}
    
	})
}
```
