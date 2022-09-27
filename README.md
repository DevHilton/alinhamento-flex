<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
 <style> 
 body{
    font-family: Arial, sans-serif;
    background-image:linear-gradient(to right, rgb(20,147,220), rgb(17,54, 71));
 }  
  .box{
    position: absolute;    
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background-color: rgba(0, 0, 0, 0.8);
    padding: 15px;
    border-radius: 15px;
   width:20% ;
   color: white;
  }
fieldset{
    border: 1px solid   dodgerblue;
}
legend{
    border: 1px solid dodgerblue;
    padding: 10px;
    text-align: center;
    background-color: dodgerblue;
    border-radius: 8px;

}
.inputBox{
    position: relative;
}
.inputUser{
    background: none;
    border: none;
    border-bottom:1px solid white ;
    outline: none;
    color: white;
    font-size: 15px;
    width: 100%;
    letter-spacing: 2px;
    color: white;
}
.inputUser:focus ~ .labelInput{
top: -20px;
font-size: 12px;
color: dodgerblue;
}
.labelInput{
    position: absolute;
    top: 0px;
    left: 0px;
    pointer-events: none ;
    transition:  0.5s;
}


 </style>
</head>
<div class="box">
<body>
<div class="flex-container">
    <form action="">
        <fieldset>
        <legend><b>Fórmulario de Cliente</b></legend>  
        <br>     
                <div class="inputBox">
                <input type="text" name="nome" id="nome" class="inputUser" required>
                <label for="nome" class="labelInput">Nome Completo</label>
            </div>
            <br>
             <div class="inputBox">                
                 <input type="text" name="email" id="email" class="inputUser" required>
                <label for="email" class="labelInput">Email</label>
                </div>
                <br>
                <div class="inputBox">
                    <input type="tel" name="telefone" id="telefone" class="inputUser" required>
                    <label for="telefone" class="labelInput">Telefone</label>
                </div>
                <br>
                <p>Sexo:</p>
                <input type="radio" id="masculino" name="genero" name="genero" value="masculino"required>
                <label for="masculino">Masculino</label>                
                <input type="radio" id="feminino" name="genero" name="genero" value="feminino"required>
                <label for="feminino">Feminino</label>
                <input type="radio" id="outros" name="genero" value="outros"required>
                <label for="outros">Outros</label><br><br>

                <div class="inputBox">
                     <label for="data_nascimento"><b>Data de Nascimento:</b></label>
                    <input type="date" name="data_nascimento" id="data_nascimento" class="inputUser" required>                   
                </div><br>
                <div class="inputBox">
                    <input type="text" name="cidade" id="cidade" class="inputUser" required>
                    <label for="cidade" class="labelInput">Cidade</label>
                </div><br>
                <div class="inputBox">
                    <input type="text" name="estado" id="estado" class="inputUser" required>
                    <label for="estado" class="labelInput">Estado</label>
                </div><br>
                <div class="inputBox">
                    <input type="text" name="endereco" id="endereco" class="inputUser" required>
                    <label for="endereco" class="labelInput">Endereco</label>
                </div><br>
                <div class="inputBox">
                    <input type="cep" name="cep" id="cep" class="inputUser" required>
                    <label for="cep" class="labelInput">Cep</label>
                </div>
                <br>
                <input type="submit" name="submit" id="submit">

               
        </fieldset>
    </form>
</div>
</div>
</body>
</html>
