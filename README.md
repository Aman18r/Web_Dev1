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




//2ND Assignment
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login Page</title>
    <style>
        body{
            background-color: black;
            color: white;
            font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
        }
        .container{
            width: 400px;
            margin: 0 auto;
            padding: 20px;
            background-color: white;
            border-radius: 5px;
            margin-top: 100px;
        }
        h1{
            color: black;
            text-align: center;
        }
        input,label{
            color: black;
        }

        .form-group{
            margin-bottom: 20px;
        }
        .form-group label{
            display: block;
            margin-bottom: 5px;
        }
        .form-group input{
            width: 100%;
            padding: 8px;
            border: 1px solid black;
            border-radius: 3px;
        }
        .form-group select{
            width: 100%;
            padding: 8px;
            border: 1px solid black;
            border-radius: 3px;
        }

        .form-group input[type="sunmit"]{
            background-color: black;
            color: white;
            cursor: pointer;
        }

        .form-group input[type="submit"]:hover{
            background-color: white;
            color: black;
        }
    </style>
</head>
<body>
    
    <div class="container">
        <h1>Signup</h1>
        <form>
            <div class="form-group">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>
            </div>
            <div class="form-group">
                <label for="batch">Batch:</label>
                <select name="batch" id="batch" required>
                    <option value="sigma1">Sigma 1.0</option>
                    <option value="sigma2">Sigma 2.0</option>
                </select>
            </div>
            <div class="form-group">
                <label for="age">Age:</label>
                <input type="number" id="age" name="age" required>
            </div>
            <div class="form-group">
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
            </div>
            <div class="form-group">
                <label for="password">Password:</label>
                <input type="password" id="password" name="password" required>
            </div>
            <div class="form-group">
                <input type="submit" value="Signup">
            </div>
        </form>
    </div>
</body>
</html>
