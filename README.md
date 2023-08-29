#<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PowerHouse Gym</title>
</head>
<style>
    body {
        margin: 0px;
        padding: 0px;
        background: url("gym2.jpg")no-repeat, center, center;
        height: 3000px;
    }
    .left {
        display: inline-block;
        position: absolute;
        left: 23px;
        top: 3px;
    }
    .center {
        position: absolute;
        left: 20%;
        top: 18px; 
    }
    .navbar {
        display: inline-block;
    }
    .navbar li {
        display: inline-block;
        font-size: 18px;
        font-family: 'Ubuntu', sans-serif;
    }
    .navbar li a:hover {
        text-decoration: underline;
        color: wheat;
    }
    .navbar li a {
        color: white;
        padding: 15px 25px;
        text-decoration: none;
    }
    .right {
        display: inline-block;
        position: absolute;
        right: 15px;
        top: 18px;
    }
    .left img {
        width: 80px;
        cursor: pointer;
    }
    .left h4 {
        text-align: center;
        margin: 0px;
        font-family: 'Ubuntu', sans-serif;
        color: wheat;
    }
    .btn {
        padding: 5px 2px;
        margin: 2px 2px;
        background-color: #ddd2bd;
        color: black;
        border-radius: 10px;
        cursor: pointer;
        font-family: 'Ubuntu', sans-serif;
        font-size: 15px;
        border: 2px solid black;
    }
    .container {
        border: 3px solid wheat;
        margin: 170px 35px;
        padding: 35px 50px;
        width: 30%;
        border-radius: 15px;
    }
    h2 {
        color: #ddd2bd;
        text-align: center;
        font-family: 'Ubuntu', sans-serif;
    }
    .form-group input {
        margin: 5px 45px;
        padding: 5px 100px;
        text-align: center;
        border-radius: 10px;  
        font-family: 'Belanosima', sans-serif;
        font-size: 15px;
    }
    .form-group input:hover{
        border: 3px solid wheat;
    }
    .btn2 {
        padding: 15px 10px;
        margin: 12px 54px;
        background-color: white;
        color: black;
        border-radius: 10px;
        cursor: pointer;
        font-family: 'Ubuntu', sans-serif;
        font-size: 18px;
        border: 2px solid black;
    }
    .btn3 {
        padding: 15px 10px;
        margin: 12px 5px;
        background-color: white;
        color: black;
        border-radius: 10px;
        cursor: pointer;
        font-family: 'Ubuntu', sans-serif;
        font-size: 18px;
        border: 2px solid black;
    }
    .btn2:hover {
       background-color: #ddd2bd;
    }
    .btn3:hover {
       background-color: #ddd2bd;
    }
</style>

<body>
    <header class="header">
        <div class="left">
            <img src="pngwing.com.png" alt="">
            <h4>PowerHouse</h4>

        </div>
        <div class="center">
            <ul class="navbar">
                <li><a href="#">ABOUT</a></li>
                <li><a href="#">FACILITIS</a></li>
                <li><a href="#">SERVICES</a></li>
                <li><a href="#">COMMUNITY</a></li>
                <li><a href="#">MEMBERSHIP</a></li>
            </ul>
        </div>
        <div class="right">
            <button class="btn">Call Us
                <script src="https://cdn.lordicon.com/bhenfmcm.js"></script>
                <lord-icon src="https://cdn.lordicon.com/ssvybplt.json" trigger="hover" colors="primary:black"
                    style="width:25px;height:25px">
                </lord-icon>
            </button>
            <button class="btn">Email Us
                <script src="https://cdn.lordicon.com/bhenfmcm.js"></script>
                <lord-icon src="https://cdn.lordicon.com/diihvcfp.json" trigger="hover" colors="primary:black"
                    style="width:25px;height:25px">
                </lord-icon>
            </button>
        </div>
    </header>
    <div class="container">
        <h2>Wellcome To PowerHouse</h2>
        <form action="noaction.php" name="myform" onsubmit="return validform()" method="post">
            <div class="form-group"  id="name">
                <input type="text " name="fname" required placeholder="Enter Your Name">
            </div>
            <div class="form-group" id="age">
                <input type="text" name="fage"  required placeholder="Enter Your Age ">
            </div>
            <div class="form-group" id="gender">
                <input type="text" name="fgender"  required placeholder="Enter Your Gender">
            </div>
            <div class="form-group" id="floc">
                <input type="text" name="floc" required  placeholder="Enter Your Locality">
            </div>
            <div class="form-group" id="fphone">
                <input type="text" name="fphone" required placeholder="Enter Your Phone Number">
            </div>
            <button type="submit" class="btn2">Submit</button>
            <button type="submit" class="btn3">Reset</button>
        </form>
    </div>
</body>
<script>
function validform() {
    
     let returnval =true;
     let name = document.getElementById('name').value;
     if (name.length<10) {
        alert("the length of name is to short");
        returnval =false;
     }
}
</script>
</html>
