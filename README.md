# HTML
Html/css/javascipt
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script>
        function data(){
            var a = document.getElementById("n1").value;
            var b = document.getElementById("n2").value;
            var c = document.getElementById("n3").value;
            var d = document.getElementById("n4").value;
            if(a==""||b==""||c==""||d==""){
                alert("All input firlds are mandatory");
                return false;
            }
            else if(b.length<10||b.length>10){
                alert("Mobile Number should be of 10 digits");
                return false;
            }
            else if(c!=d){
                alert("password and confirm password should be same");
                false
            }
            else{
                true;
            }
        }
    </script>
    <form onsubmit="return data()">
        User ID: <br>
        <input type="text" id="n1"> <br>
        Mobile Number: <br>
        <input type="text" id="n2"> <br>
        Password: <br>
        <input type="password" id="n3"> <br>
        Confirm Password: <br>
        <input type="password" id="n4"> <br><br>
        <input type="submit" value="submit"> <br>
    </form>
    
</body>
</html>
