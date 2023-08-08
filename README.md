# Web_Dev1

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Web Page</title>
    <style>
        *{
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body{
            font-family: Arial, Helvetica, sans-serif;
            background-color: #f1f1f1;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        .container{
            width: 400px;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        .login-box{
            padding: 40px;
        }
        h2{
            text-align: center;
            margin-bottom: 30px;
            color: #333;
        }
        form{
            display: flex;
            flex-direction: column;
        }
        .user-box{
            position: relative;
            margin-bottom: 30px;
        }

        .user-box input{
            width: 100%;
            padding: 10px 0;
            font-size: 16px;
            color: #333;
            border: none;
            border-bottom: 1px solid #333;
            outline: none;
            background: transparent;
            transition: border-color 0.2s;
        }

        .user-box label{
            position: absolute;
            top: 0;
            left: 0;
            font-size: 16px;
            color: #777;
            pointer-events: none;
            transition: all 0.2s;
        }

        .user-box input:focus ~ label,
        .user-box input:valid ~ label{
            top: -20px;
            font-size: 12px;
            color: #1e87f0;
        }

        a{
            display: inline-block;
            background-color: #1e87f0;
            color: #fff;
            text-decoration: none;
            padding: 10px 20px;
            border-radius: 5px;
            font-size: 16px;
            text-align: center;
            transition: background-color 0.2s;
        }

        a:hover{
            background-color: #1472c4;
        }
    </style>
</head>
<body>
    
    <div class="container">
        <div class="login-box">
            <h2>Login</h2>
            <form>
                <div class="user-box">
                    <input type="text" name="username" required="">
                    <label>Username</label>
                </div>
                <div class="user">
                    <input type="password" name="password" required="">
                    <label>Password</label>
                </div>
                <a href="#">
                    <span></span>
                    <span></span>
                    <span></span>
                    <span></span>
                    Submit
                </a>
            </form>
        </div>
    </div>
</body>
</html>
