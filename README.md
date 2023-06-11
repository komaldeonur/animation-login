# animation-login
login form
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Animated Login Form </title>
</head>
<body>
    <div class="form-container">
        <h2 class="login-title">login</h2>
        <input type="text" name="text" class="userName" placeholder="userName">
        <input type="password" name="password" class="userPassword" placeholder="password">
        <button class="loginBtn">Login</button>
    </div>
</body>
</html>

<!-- style.css -->

@import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;    
}
body{
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 100%;
}
.form-container{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    background: black;
    color: white;
    border-radius: 10px;
    padding: 5em 2rem;
    box-shadow: 0px 0px 20px 0px black;
    border: 1px solid black;
}
.login-title{
    font-size: 2rem;
    margin-bottom: 2rem;
}
.userName,
.userPassword {
    text-align: center;
    border: 2px solid cyan;
    margin: 1rem;
    color: white;
    background: transparent;
    padding: 1rem 2rem;
    border-radius: 3rem;
    width: 15rem;
    font-size: 1.2rem;
    outline: none;
    transition: all .2s ease-in-out;
}
.userName:focus,
.userPassword:focus{
    width: 20erm;
    animation-name: colorchange;
    animation-duration: 10s;
    animation-iteration-count: infinite;
}
@keyframes colorchange{
    0%{
        border-color: green;
        color: green;
    }
    10%{
        border-color: yellow;
        color: yellow;
    }
    20%{
        border-color: hotpink;
        color: hotpink;
    }
   30%{
        border-color: purple;
        color: purple;
    }
    40%{
        border-color: red;
        color: red;
    }
    50%{
        border-color: yellow;
        color: yellow;
    }
    60%{
        border-color: cyan;
        color: cyan;
    }
    70%{
        border-color: skyblue;
        color: sk;
    }
    80%{
        border-color: pink;
        color: pink;
    }
    90%{
        border-color: red ;
        color: red;
    }
    100%{
        border-color: yellow;
        color: yellow;
    }
}
.loginBtn
{
    background-color: transparent;
    border: 2px solid green;
    padding: 1rem 3rem;
    border-radius: 6rem;
    text-decoration: underline;
    font-size: 1rem;
    cursor: pointer;
    transition: all .3s ease-in-out;
    color: white;
}
.loginBtn:hover{
    background: green;
    border: 2px solid green;
}
