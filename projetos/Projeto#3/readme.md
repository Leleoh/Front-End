Aqui deixarei registrados as dificuldades e observações encontradas na criação do projeto e como é a solução, caso seja encontrada

---DICAS---
*Antes de começar a criar a página, pode "zerar" as formatações existentes nela
*É possível usar a mesma formatação em diferentes ids e classes, para fazer isso basta colocar uma vírgula após cada id/class Ex: #cabecalho, #menu{}

#Problema 1: Deixar o cabeçalho do site sem margens em relação à página, tirando o espaçamento branco em cima e dos lados.
Solução: Foi possível fazer isso antes mesmo de começar o projeto, "zerando" as formatações pré-existentes no documento, setando as margens e espaçamentos para 0 com o seletor *

#Problema 2: Dar espaçamento entre o logo "TECBLOG" e os menus abaixo do mesmo
Solução: Na ID do logo foi só utilizar o padding bottom, e depois setar o valor desejado que o espaço foi aplicado

#Problema 3: Personalizar o logo "TecBlog", com cores diferentes para cada parte e tamanho diferente.
Solução: Para fazer isso criei um seletor exclusivo para o h1, onde apliquei uma cor e um tamanho; Para fazer cada parte com uma cor foi necessário criar uma nova classe com a cor branca e depois separálos no html, para depois de tudo juntar novamente com o span, aplicando a classe .branco no span

#Problema 4: Formatar os links de mandeira que se adaptem ao projeto.