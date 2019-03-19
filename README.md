# suitable
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=UTF-8" />
<title>Test5</title>
<script type="text/javascript">
    function operation(){
	    //第一个数
	    var oneNumber =  parseInt(document.getElementById("one").value);
		//第二个数
		var twoNumber =  parseInt(document.getElementById("two").value);
		//运算符
		var calculate = document.getElementById("fuhao").value;
		//计算结果
		var result = parseInt(document.getElementById("fuhao").value);

		switch(calculate)
		{
		    case'+':result = oneNumber + twoNumber;
			     break;
			
			case'-':result = oneNumber - twoNumber;
			     break;
			
			case'*':result = oneNumber * twoNumber;
			     break;
			
			case'/':result = oneNumber / twoNumber;
			    break;
				
			default:alert("错误");
			    break;
		}
		var result1=document.getElementById("result1");
		result1.value =result;		
	}
</script>
</head>
<body>
   <input type="text" id="one" size="12" style="width:40px; "/>
   <input type="text" id="fuhao" size="12" style="width:40px; "/>
   <input type="text" id="two" size="12" style="width:40px; "/> =
   <input type="text" id="result1" size="12" style="width:40px; "/>
   <input type="button"  value="计算"  onclick="operation();"/>
</body>
</html>
