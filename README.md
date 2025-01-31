O HTML é uma linguagem de marcação.
Se você colocar ! no início do projeto a página irá fazer a estrutura básica do html.

<!DOCTYPE html>

línguagem (no caso usamos a pt-br)
<html lang="pt-br">

<head>
    caracteres
    <meta charset="UTF-8">

    faz com que a página esteja sempre em sua versão mais recente no Internet Explorer
    <meta http-equiv="X-UA-Compatible" content="IE=edge">

    adaptar os tamanhos de acordo com a escala do aparelho
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    título da página, ainda na barra
    <title>Portifólio</title>

    linkar o html com o CSS
    <link rel="stylesheet" href="style.css">

</head>
<body>
    cabeçalho
    <header></header>(tag semântica)

    corpo
    <main> (tag semântica)
        título, 'texto maior'
        <h1>AQUI</h1>

        parágrafo, 'texto menor'
        <p>AQUI</p>

                para deixar o texto destacado utiliza-se a tag strong ou span. 
                A strong irá deixar o texto em negrito e você pode mudar a cor no CSS(1). Pode ser <strong> ou 3 <strong class="descrição">
                A span deixará em aberto diversas funcionalidades, deixando o texto mais estilizável (2).

        link, redirecionar
        <a href="link">AQUI</a> (tag âncora)

        colocar imagem
        <img src=img.png alt="Descreva a imagem">
    </main>(tag semântica)

    rodapé
    <footer></footer>(tag semântica)
</body>
</html>

O CSS é uma linguagem de estilização, é como o html deve ser exibido na tela.

O atalho * seleciona todos os conteúdos.

*{
  (define que não terá margem)
  margin: 0;

  (define que não terá espaço entre borda e conteúdo)
  padding: 0;
}

body {

(muda a altura do conteúdo)
height= 100vh;

(ajusta a largura do conteúdo para que não saia do limite estabelecido, para saber mais: https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing)
box-sizing: border-box;

(muda a cor de fundo)
  background-color: rgb(56, 19, 109); 

(muda a cor da fonte)
  color: #códigodacor;
}

1 (muda a cor do texto entre a tag strong)
strong {
    color: #códigodacor;
}
(se tiver mais de um strong é necessário atribuir uma classe a ele, isso se faz no HTML3)
.nomeDaClasse {
  color: #códigodacor;
}

2 (estiliza o texto da tag span)
span{
        (texto em negito, pode ser outras maneiras ex: italic)
        font-weight: bold;

        (cor do texto)
        color: #códigodacor;

        (coloca uma borda colorida no texto)
        border: 1px solid #códigodacor;

        (define o espaçamento interno)
        padding: 10px;
}