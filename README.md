# Fortune Cookie

Este README fornece uma visão geral do código HTML e JavaScript fornecido para um aplicativo da web "Fortune Cookie". O código tem como objetivo criar uma página da web simples que simula a experiência de abrir um biscoito da sorte e exibir uma mensagem aleatória.

## Tabela de Conteúdo

- [Visão Geral](#visão-geral)
- [Estrutura de Arquivos](#estrutura-de-arquivos)
- [Uso](#uso)
- [Funcionalidade](#funcionalidade)
- [Notas Adicionais](#notas-adicionais)

## Visão Geral

O código fornecido é uma página HTML que imita a experiência de abrir um biscoito da sorte. Ela exibe uma imagem de um biscoito da sorte fechado e um botão. Quando o botão é clicado, uma animação é acionada, simulando a abertura do biscoito. Após um curto atraso, uma mensagem aleatória é buscada de um servidor (assumindo que o servidor está em execução em `http://localhost:8080/phrases`) e a mensagem é exibida em um pop-up modal. O modal pode ser fechado clicando em qualquer lugar da tela.

## Estrutura de Arquivos

- `index.html`: O arquivo HTML principal que contém a estrutura da página da web, incluindo o cabeçalho, imagem do biscoito da sorte, botão e modal.
- `style.css`: O arquivo CSS vinculado ao HTML para estilizar a página da web.
- `img/`: Uma pasta contendo as imagens usadas no aplicativo.
- `script.js`: Código JavaScript inline incluído no arquivo HTML para gerenciar a interação e funcionalidade da página da web.

## Uso

Para usar este código:

1. Coloque o código HTML, CSS e JavaScript fornecido em seus respectivos arquivos (`index.html`, `style.css` e `<script>` inline no HTML).
2. Certifique-se de ter as imagens necessárias (`biscoito-da-sorte.png`, `biscoito.png` e `cookiee-animation.gif`) dentro da pasta `img/`.
3. Se você planeja usar a funcionalidade de busca no servidor para obter frases aleatórias, verifique se seu servidor está em execução e configurado corretamente para responder a solicitações em `http://localhost:8080/phrases`.

## Funcionalidade

1. O cabeçalho inclui um logotipo ("Fortune Cookie") e links de navegação para "Inicio" e "Sorte".
2. Clicar no botão "Abrir Biscoito" aciona as seguintes ações:
   - A imagem do biscoito da sorte muda para um GIF animado que representa a abertura do biscoito.
   - O botão é ocultado.
   - Uma requisição fetch é feita para o endpoint do servidor especificado (`http://localhost:8080/phrases`) para recuperar uma mensagem aleatória.
   - A mensagem recuperada é exibida em um pop-up modal após um breve atraso.
3. O pop-up modal tem uma funcionalidade de fechamento, acionada ao clicar em qualquer lugar da tela enquanto o modal está aberto.

## Notas Adicionais

- Este é um exemplo simplificado e não inclui a implementação real do servidor para fornecer frases aleatórias. Verifique se você tem um servidor em execução no endpoint especificado para buscar mensagens.
- O código usa JavaScript puro para simplificar, mas em um aplicativo do mundo real, você pode considerar o uso de um framework como React, Vue ou Angular para melhor estrutura e manutenibilidade.
- A estilização fornecida em `style.css` é mínima. Você pode aprimorar o design e o layout de acordo com suas preferências.
- O código pressupõe que `cookiee-animation.gif` é uma imagem animada que simula a abertura do biscoito da sorte.
- Os comentários e a lógica do código foram organizados para facilitar o entendimento, mas você pode documentar e modularizar ainda mais o código para melhor legibilidade e manutenibilidade.