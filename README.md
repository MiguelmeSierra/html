<html>
    <head>
        <meta charset="UTF-8">
        
        <title>Miguel DS102</title>
        <style>
            body{
                background: rgb(228, 214, 88);
            }



        
        
        </style>
    </head>
    <body>
        <h1>Cadastramento</h1>
        <br>nome:<input id="nome" type="text"></input>
        <br></br>
        <br>sobrenome:<input id="sobrenome" type="text"></input>
        <br></br>
        <br>idade:<input id="idade" type="number" maxlength="2"></input>
        <br></br>
        <br>cidade:<input id="cidade" type="text"></input>
        <br></br>
        <br>estado:<input id="estado" type="text" maxlength="2"></input>
        <br></br>
        <p id="p1"></p>

        <button onclick="enviar()">Enviar</button>
        <script>
            function enviar(){
            var nome = document.getElementById('nome').value;
            var sobrenome = document.getElementById('sobrenome').value;
            var idade = document.getElementById('idade').value;
            var cidade = document.getElementById('cidade').value;
            var estado = document.getElementById('estado').value;
            var nomeCompleto = nome+' '+sobrenome+' tem '+idade+ ' anos,'+ ' e mora em'+' '+ cidade+ '/'+ estado;
            document.getElementById('p1').innerHTML = nomeCompleto;
            } 
        
        
        </script>
    </body>





</html>
