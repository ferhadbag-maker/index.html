<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Instagram Login</title>

<style>
body{
    margin:0;
    font-family: Arial, Helvetica, sans-serif;
    background: linear-gradient(180deg,#0a0f14,#0f2a33);
    height:100vh;
    display:flex;
    justify-content:center;
    align-items:center;
    color:white;
}

.container{
    width:350px;
}

.logo{
    text-align:center;
    font-size:28px;
    margin-bottom:30px;
}

h2{
    font-size:20px;
    margin-bottom:20px;
}

input{
    width:100%;
    padding:14px;
    margin:8px 0;
    border-radius:10px;
    border:1px solid #2b3e46;
    background:#0e1f26;
    color:white;
}

input::placeholder{
    color:#9aa4aa;
}

.login-btn{
    width:100%;
    padding:14px;
    margin-top:10px;
    border:none;
    border-radius:25px;
    background:#1f5fbf;
    color:white;
    font-weight:bold;
    cursor:pointer;
}

.login-btn:hover{
    background:#1a53a6;
}

.forgot{
    text-align:center;
    margin:15px 0;
    font-size:14px;
}

.fb-btn{
    width:100%;
    padding:12px;
    border-radius:25px;
    border:1px solid #3b5998;
    background:transparent;
    color:white;
    cursor:pointer;
}

.create{
    width:100%;
    padding:12px;
    margin-top:15px;
    border-radius:25px;
    border:1px solid #2a6df4;
    background:transparent;
    color:#4ea1ff;
    cursor:pointer;
}

.meta{
    text-align:center;
    margin-top:25px;
    color:#9aa4aa;
    font-size:14px;
}
</style>

</head>

<body>

<div class="container">

<div class="logo">Instagram</div>

<h2>Log into Instagram</h2>

<input type="text" placeholder="Mobile number, username or email">
<input type="password" placeholder="Password">

<button class="login-btn">Log in</button>

<div class="forgot">Forgot password?</div>

<button class="fb-btn">Log in with Facebook</button>

<button class="create">Create new account</button>

<div class="meta">Meta</div>

</div>

</body>
</html>
