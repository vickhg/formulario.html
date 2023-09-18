<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulario | GN</title>
    <style>
        body{
        font-family: Arial, Helvetica, sans-serif;           
        background: linear-gradient(#d1000a, #6e2525);
        /*background: #FFFFFF;*/ 
        }
        .box{
        color: white;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%,-50%);
        background-color:black;
        padding: 15px;
        border-radius: 15px;
        width: 20%;
        }
        fieldset{
        border: 3px solid dodgerblue;
        }
        legend{
        border: 1px solid dodgerblue;
        padding: 10;
        text-align: center;
        background-color: dodgerblue;
        border-radius : 8px;
        }

        .inputbix{
        position: relative;

        }  
        .inputUser{
        background: none;
        border: none;
        border-bottom: 1px solid white;
        outline: none;
        color: white;
        font-size: 15px;
        width: 100%;
        letter-spacing: 2px;
        }
        labelInput{
        position: absolute;
        top: 0px;
        left: 0px;
        pointer-events: none;
        transition: .5s;
        }
    </style>
</head>
<body>
    <div class="box">
        <form action="processa.php" method="get">
            <fieldset>      
                <legend><b>Formulario de Clientes</b></legend>
                <br>
                <div class="inputbox">
                    <input type="text" name="nome" id="nome" class="inputUser" required>
                    <label for="nome" class="labelInput">Nome Completo</label>
                </div>
                <br>
                <div class="inputbox">
                    <input type="text" name="email" id="email" class="inputUser" required>
                    <label for="email" class="labelInput">E-mail</label>
                </div>
                <br>
                <div class="inputbox">
                    <input type="text" name="email" id="email" class="inputUser" required>
                    <label for="telefone" class="labelInput">Telefone</label>
                </div>
                <br>
                    <p>Sexo:</p>
                    <input type="radio" id="feminino" name="genero"value="feminino" required>
                    <label for="feminino">Feminino</label>
                    <input type="radio" id="masculino" name="genero"value="masculino" required>
                    <label for="masculino">Masculino</label>
                    <input type="radio" id="outro" name="genero"value="outro" required>
                    <label for="outro">Outro</label>
                <br><br>            
                <div class="inputbox">
                    <label for="data_nacimento"><b>Data de Nacimento:</b></label>
                    <input type="date" name="data_nacimento" id="data_nacimento" class="inputUser" required>
                </div>
                <br>
                <div class="inputbox">
                    <input type="text" name="Cidade" id="Cidade" class="inputUser" required>
                    <label for="cidade" class="labelInput">Cidade</label>
                </div>
                <br>
                <div class="inputbox">
                    <input type="text" name="estado" id="estado" class="inputUser" required>
                    <label for="estado" class="labelInput">Estado</label>
                </div>
                <br>
                <div class="inputbox">
                    <input type="text" name="endereco" id="endereco" class="inputUser" required>
                    <label for="endereco" class="labelInput">Endereço</label>
                </div>
                <br> 
                <input type="submit" name="submit" id="Salvar">
                <input type="reset" name="submit" id="Limpar">
            </fieldset>
        </form>
    </div>
</body>
</html>
