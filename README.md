# htmlcode1
code for form validation
<html>
<head>
    <title> Legal Advisory </title> 
    <style>
    	body{
    		background-repeat: no-repeat;
    		background-size: cover;
    		background-position: center;
    	}
    </style>

 </head>
<body bgcolor = "sky blue">
   	
     <H1><center><b><i>Welcome to advisory site</i></b></center></h1>
	  <input type = "button" value ="click" onclick = "myfunction()">  
	  <div id="dt">hello</div>
	  <br>Enter Color of your choice <input type="text" id="ty"><br><br>
	
	  <input type = "button" value = "changecolor" onclick = "changecolor()">
	  <script>
     console.log("hello world") 
	 function myfunction()
	 {   
	    var name = document.getElementById("dt");
		 var abc = prompt("enter your name");
		//alert(name.innerHTML);
		name.innerHTML += "hi" +abc+ "welcome";
	 }
	  function changecolor()
	 {
	   var tb= document.getElementById("dt");
	   var ty=document.getElementById('ty').value;
	   tb.style.color = ty;
	 }
	 function verify()
	 {
	  var x = document.getElementByName("array[]");
	  for(var i =0;i<x.length;i++)
	  {
	  var a = x[i].value;
	  console.log(a);
	  if(a=="")
	  {
	  alert("mandatory field left out");
	  return false;
	  }
	  i++;
	  }
	  var p1 = document.getElementById("p1").value;
		var p2 = document.getElementById("p2").value;
		if(p1!=p2)
		{
		  alert("password error");
		  return false;
		}
	 }
		 
</script>
	 <h1><font color = blue> please enter your bio data </h1>
 <form name = "form1" method = "get" action = "https://uppsc.up.nic.in/"  onsubmit = "return verify()">
     First name : <input type="text" name = "array[]" size = "15" maxlength="25"><br>
     Last name : <input type = "text" name="array[]" size = "15 maxlength = "25"><br>
     Email Id : <INPUT type ="text" name ="array[]" size= "15" maxlength="25"><br>
     Password : <input id = "p1" type = "password" name="array[]" size= "15" maxlength = "10"><br>
     confirm password: <input id = "p2" type= "password" name="array[]" size = "15" maxlength ="25"><br>
	 submit : <input type="submit" name= "submitbutton" size = "15"><br>
	 
 
 </body>
 </html>
