# Tutorial:Criação da estrutula de Layout de um Chat

Neste tutorial, vou mostrar a você como criar uma página HTML simples para criar um layout de um chat. O código HTML que você forneceu é uma estrutura de exemplo que pode ser usada como ponto de partida.

## Pré-requisitos

Antes de começar, certifique-se de ter um editor de texto, como o Visual Studio Code, Sublime Text ou qualquer outro de sua escolha, instalado em seu computador.

### Passo 1: Estrutura Básica

Comece com a estrutura básica do HTML, que inclui a declaração do tipo de documento, o elemento `<html>`, o `<head>` e o `<body>`.

```html
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gama Chat</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/css/materialize.min.css">
    <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
    <link rel="stylesheet" href="./css/style.css">
</head>
<body>
    <!-- Conteúdo da página -->
</body>
</html>
```

### Passo 2: Cabeçalho

No corpo da página, crie um cabeçalho `<h1>` com o título "Gama Chat".

```html
<div class="container">
    <h1 class="center">Gama Chat</h1>
</div>
```

### Passo 3: Caixa de Chat

Crie um elemento `<div>` com a classe "chatbox" para conter as mensagens. Dentro dessa caixa, adicione as mensagens de erro, usuário e bot como `<div>`s com as classes apropriadas.

```html
<div id="chatbox" class="z-depth-1">
    <!-- Mensagens vão aqui -->
    <div class="message error-message">
        <div class="message-content">
            <img class="avatar" src="assets/bot.png">
            <p>Mensagem de erro</p>
        </div>
    </div>
    <div class="message user-message">
        <div class="message-content">
            <img class="avatar" src="assets/bot.png">
            <p>Mensagem de usuário</p>
        </div>
    </div>
    <div class="message bot-message">
        <div class="message-content">
            <img class="avatar" src="assets/bot.png">
            <p>Mensagem do bot</p>
        </div>
    </div>
</div>
```

### Passo 4: Barra de Progresso

Adicione uma barra de progresso com a classe "progress" para indicar que algo está acontecendo em segundo plano.

```html
<div class="progress">
    <div id="loading"></div>
</div>
```

### Passo 5: Formulário de Chat

Crie um formulário com o ID "chatForm" que inclui um campo de entrada de texto e um botão para enviar mensagens. O botão possui um ícone "send" usando o Material Icons.

```html
<form id="chatForm">
    <input type="text" name="messageInput" id="messageInput" placeholder="Digite sua mensagem...">
    <button type="submit" class="btn-floating btn-large waves-effect waves-light green">
        <i class="material-icons">send</i>
    </button>
</form>
```

### Passo 6: Scripts

No final do corpo da página, você pode incluir scripts para funcionalidade adicional. No exemplo fornecido, você já incluiu o JavaScript da biblioteca Materialize.

```html
<!-- Compiled and minified JavaScript -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/materialize/1.0.0/js/materialize.min.js"></script>
```

Certifique-se de que você tenha os arquivos CSS e as imagens necessárias (bot.png) na pasta correspondente para que a página funcione corretamente. Este é um exemplo básico de uma página de chat que pode ser estilizada e programada para interagir com um chatbot ou sistema de mensagens.
