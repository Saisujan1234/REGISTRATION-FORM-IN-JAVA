# REGISTRATION-FORM-IN-JAVA

<html>
<head>
<script>
function validateform(){
var uname=document.myform.uname.value;
var pwd=document.myform.pwd.value;
if(uname.length==0){
 alert("Please enter a Username");
 return false;
}
if(pwd.length<6){ 
  alert("Password cannot less than 6 characters");
  return false;
 }
return true;
 }
</script>
</head>
<body>
<h1> Login Form </h1>
<form name="myform" onsubmit="return validateform()">
<table>
<tr><td>Name:</td>
<td><input type="text" name="uname"></td>
</tr>
<tr><td>Password:</td>
<td><input type="Password" name="pwd"></td>
</tr>
<tr><td><input type="submit" value="submit"></td></tr>
</table>
</form>
</body>
</html>


<html>
<body>
    <h2>Registration form</h2>
    <form>
    <label for="reg">Username:</label><br>
    <input type="text" class="regno"><br>
    <label for="reg">Password:</label><br>
    <input type="password" class="Pass"><br>
    <label for="email">SRM email id :</label><br>
    <input type="text" class="Email"><br>
    <label for="phone">Mobile number:</label><br>
    <input type="number" class="mobile"><br>
    <br>
    <input type="submit" value="Submit" class="Login">	
</form>


<script>
const lgn = document.querySelector('.Login')
lgn.addEventListener("click", Run);
function Run(e)
{
const email = document.querySelector('.Email').value
const pass = document.querySelector('.Pass').value
const user = document.querySelector('.regno').value
const number = document.querySelector('.mobile').value

if(email.includes("@srmist.edu.in") && pass.length >=8 && user.length >=4 && number.length === 10)
{
alert("Registration Successful")
}
else
{
alert("Invalid Credential")
}
}
</script>
</body>
</html>
