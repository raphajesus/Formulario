# Formulario
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Form contato</title>
</head>
<style>
    *{margin: 0; padding: 0;box-sizing: border-box;}
    body{
        background-color: #5F7C8A;
    }

    form{
        background-color: white;
        max-width: 500px;
        width: 70%;
        padding: 20px;
        position: absolute;
        left: 50%;
        top: 50%;
        transform: translate(-50%,-50%);
    }

    form h3{
        text-align: center;
        color: #5F7C8A;
        font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    }

    form input[type=text],
    form input[type=password]{
        width: 100%;
        height: 45px;
        border: 1px solid #ccc;
        padding-left: 10px;
        margin:10px 0;

    }
       form input[type=submit]{
        width: 100%;
        height: 30px;
        cursor: pointer;
        background:#5F7C8A ;
        color: white;
        border: 0;
        border-radius: 20px;
        transition: 1s;
       }

       form input[type=submit]:hover{
        background-color: #4A5F6A;
       }

       
        form input[type=text]:focus{
            outline: 0;
       
       }
       form input[type=password]:focus{
            outline: 0;
       
       }
</style>

<form>
    
     <form>
        <h3>Entrar em contato</h3>
      <input id="email" type="text" name="email" placeholder="Seu e-mail..."/>
        <input id="password" type="password" name="senha" placeholder="Sua senha.."/>
          <input type="submit" name="acao" value="enviar"/>
        </form>

        <script>

            var email = document.getElementById('email');
            var password = document.getElementById('password');
             
            email.addEventListener('focus',()=>{
                email.style.borderColor = "#4A5F6A";
            });

            email.addEventListener('blur',()=>{
                email.style.borderColor = "#ccc";
            });

            password.addEventListener('focus',()=>{
                password.style.borderColor = "#4A5F6A";
            });

            password.addEventListener('blur',()=>{
                password.style.borderColor = "#ccc";
            });

        </script>

          </body>
             </html>
