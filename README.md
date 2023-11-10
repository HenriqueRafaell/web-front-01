# web-front-01
git status- pra saber o que eu to fazendo 
git add . pra adicionar
git comit -m"adicionado aqrquivo"
git push origin nome_hrach - pra subir o arquivo


CABEÇALHO DE DO JAVASCRIPT
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    
</body>
</html>

html giovani dia 10/11

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contato</title>
    <link rel="stylesheet" href="./css/style.css">
</head>
<body>
    <div class="contaiener">
        <form action="">
            <div class="form-control">
                <input type="text" id="nome" placeholder="Digite seu nome">
            </div>
            <div class="form-control">
                <input type="text" id="cidade" placeholder="Digite sua cidade">
            </div>

            <div>
                <button type="submit">Enviar</button>
            </div>
        </form>

        <div class="lista">
            <ul class="remedios"></ul>
            <button class="">Mostra Medicamentos</button>
            <ul class="remedios">
                <li>Dorflex</li>
                <li>Lorem</li>
                <li>Dipirona</li>
            </ul>
        </div>

    </div>

    <script src="./js/script.js"></script>
</body>
</html>


script 

const buttonMedicamentos = document.querySelector("#medicamentos");
const remedios = document.querySelector(".remedios")

//variavel validaçao

const campoNome = document.querySelector("#nome")
const campoCidade = document.querySelector("Cidade")
const buttonEnviar = document.querySelector("button")



//função da validação 
buttonEnviar.addEventListener("click", function(event){
    event.preventDefault();
    if (campoNome.value === ''){
        alert("preencha o campo nome")

    ;
    return false
    }

    if (campoCidade.value === ''){
        alert("preencha o campo cidade")
        return false;

    }

function clearForm(){
    campoNome.value = "";
    campoCidade.value = "";
}

})


buttonMedicamentos.addEventListener("click",function(){
    remedios.classList.add("d-block")

})

css


*{
    list-style: none;
    
}

body{
    background-color: antiquewhite;
}

.contaiener{
    border: 1px solid black;
    max-width: 500px;
    margin: 20px auto;
    background: #fff;
    border-radius: 5px;
    text-align: center;
}

.form-control{
    margin: 25px;
}

.form-control input[type="text"]{
    width: 80%;
    padding: 10px;
    outline: 0;

}

button{
    margin-bottom: 20px;
    background-color: blueviolet;
    border: 0;
    padding: 10px;
    color: #fff;
    cursor: pointer;
    font-size: 15px;
}

.erro{
    color: red;
    text-align: left;
    margin-left: 32px;

}

.d-none{
    display: none; 

}

.d-block{
    display: block;
}


