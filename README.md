Exercícios de HTML e JavaScript

Coleção de pequenos exercícios de estudo em HTML, CSS e JavaScript. Cada arquivo é uma página independente: basta abri-la em um navegador. Não há dependências nem instalação.

Estrutura dos arquivos
Arquivo	Tema	Descrição
ex001.html	Entrada de dados	Exibe um prompt pedindo o nome do usuário.
ex002.html	Entrada e saída	Pede o nome, mostra um alert de boas-vindas e escreve a mesma mensagem na página.
ex003.html	Operações matemáticas	Pede dois números, soma-os e mostra o resultado em um alert.
ex004.html	Comparação lógica	Soma dois valores fixos e exibe se o resultado é maior ou igual a 5.
ex005.html	Introdução ao DOM	Seleciona elementos com document.querySelector e altera estilo e texto.
ex006.html	Eventos do DOM	Muda a cor e o texto de uma caixa ao clicar, passar o mouse e sair dela.
ex006p2.html	Formulário simples	Campos numéricos e botão para somar os valores digitados.
ex007.html	—	Arquivo vazio.
snsd.html	—	Arquivo vazio.
Como executar
Baixe ou copie o arquivo .html desejado.
Dê dois cliques nele, ou abra-o com o navegador (Chrome, Firefox, Edge etc.).
Para exercícios com prompt e alert, responda às janelas que aparecerem.
Detalhes por exercício
ex001.html: Olá, mundo!
Define estilo do body (fundo azul, texto branco, fonte Arial 20pt).
Exibe o título e um parágrafo fixos.
Executa window.prompt("Digite seu nome?"), mas não guarda nem mostra a resposta.
ex002.html: Recebendo o nome
Guarda a resposta do prompt na constante nome.
Mostra alert com a saudação usando template string (`Ola ${nome}`).
Preenche o parágrafo #nome com a mesma saudação via innerText.
ex003.html: Soma de dois números
Pede dois números com prompt.
Converte os textos para número com Number() e soma.
Exibe o total em um alert e escreve, no <h2> com id="a1", o texto mostra esse valor not, a partir da constante n3.
ex004.html: Comparação
Declara a = 3 e b = 2 e calcula c = a + b.
Mostra um alert com o resultado da comparação c >= 5.
Resultado esperado: true, pois 3 + 2 = 5, e 5 é maior ou igual a 5.
A <div id="a1"> está vazia e não é usada.
ex005.html: DOM
Usa document.body e document.getElementsByTagName("p") para selecionar elementos.
Usa document.querySelector("div#msg") para selecionar a caixa de texto.
Altera o fundo para azul e o texto para "Estou aguardando...".
O código contém alternativas comentadas (getElementsByName, getElementsByClassName) que servem como referência.
ex006.html: Eventos
A <div id="area"> responde a três eventos:
Clique: texto "Clicou!" com fundo vermelho.
Mouse entra: texto "Entrou!" com fundo azul.
Mouse sai: texto "Saiu!" com fundo verde.
Os eventos são definidos de duas formas ao mesmo tempo: atributos HTML (onclick, etc.) e addEventListener. Veja o item "Problemas conhecidos".
ex006p2.html: Somando valores
Dois campos numéricos (#txtn1 e #txtn2) e um botão "Somar".
Ao clicar, a função somar() lê os valores, soma-os e mostra o resultado na div#res.
Veja o item "Problemas conhecidos" sobre o campo de seleção.
Problemas conhecidos

Alguns pontos que podem ser corrigidos nos exercícios:

ex006.html: cada evento está registrado duas vezes (atributo HTML e addEventListener), então a função roda duas vezes a cada ação. Basta manter apenas um dos dois métodos.
ex006p2.html: dentro de somar(), a variável tn2 usa #txtn1 no seletor, quando deveria ser #txtn2. Assim, a soma usa sempre o primeiro campo duas vezes.
ex006p2.html: o atributo type="caixa" não é um tipo de input válido e não tem efeito. Além disso, a tag </body> está ausente.
ex001.html: o nome digitado no prompt não é usado.
ex003.html: a constante n3 é fixa ("not"), então a frase exibida não depende de nenhuma entrada do usuário.
ex005.html: a variável p1 é declarada, mas não é utilizada.
Tecnologias
HTML5
CSS (estilos embutidos na tag <style>)
JavaScript (código embutido na tag <script>)
Caixas de diálogo do navegador: prompt e alert
