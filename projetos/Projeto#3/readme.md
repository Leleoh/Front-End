Aqui deixarei registrados as dificuldades e observações encontradas na criação do projeto e como é a solução, caso seja encontrada

---DICAS---
*Antes de começar a criar a página, pode "zerar" as formatações existentes nela
*É possível usar a mesma formatação em diferentes ids e classes, para fazer isso basta colocar uma vírgula após cada id/class Ex: #cabecalho, #menu{}
*SEMPRE faça comentários no CSS EXTERNO organizando as coisas
*É possível fazer comentários de começo e fim para organizar o código

#Problema 1: Deixar o cabeçalho do site sem margens em relação à página, tirando o espaçamento branco em cima e dos lados.
Solução: Foi possível fazer isso antes mesmo de começar o projeto, "zerando" as formatações pré-existentes no documento, setando as margens e espaçamentos para 0 com o seletor *

#Problema 2: Dar espaçamento entre o logo "TECBLOG" e os menus abaixo do mesmo
Solução: Na ID do logo foi só utilizar o padding bottom, e depois setar o valor desejado que o espaço foi aplicado

#Problema 3: Personalizar o logo "TecBlog", com cores diferentes para cada parte e tamanho diferente.
Solução: Para fazer isso criei um seletor exclusivo para o h1, onde apliquei uma cor e um tamanho; Para fazer cada parte com uma cor foi necessário criar uma nova classe com a cor branca e depois separálos no html, para depois de tudo juntar novamente com o span, aplicando a classe .branco no span

#Problema 4: Formatar os links de mandeira que se adaptem ao projeto.
Solução: Para isso eu criei uma nova área exclusiva de formatações de links, a fim de tornar o código mais organizado. Comecei criando dois seletores para o link a:link, com a propriedade color, o que mudou a cor dos links estáticos. Após isso a:hoover, com color e background em cores adequadas, o que possibilitou fazer a formatação quando o mouse passa em cima.
Estilos que apliquei nos links: color, background-color, padding, text-decoration

#Problema 5: Criar uma estrutura com tamanho fixo para mostrar as postagens recentes abaixo do cabeçalho.
Solução: Criei uma nova área de layout, com background, width e margin para dar o espaçamento

#Problema 6: Criar uma área separada do layout principal com as postagens.
Solução: Duas novas divs separadas foram criadas dentro da div principal, uma exclusiva para a área de postagens e outra para a área lateral que deveria ser criada.
-Removi o bg da área principal, já que agora ele vai ser aplicado diretamente nessas duas novas divs
-Criei dois novos ids na parte do layout, configurei tamanhos distintos, cores para o bg, tudo separado para cada uma.
-Tive de usar uma tag de elementos flutuantes, a tag float, para poder tirar um de baixo do outro e posicionar a esquerda/direita

#Problema 7: Criar um rodapé
Solução: Na div principal criei abaixo das outras duas áreas, a área do rodapé, usei um clear para separá-lo das outras duas divs, e algumas tags de formatação para personalizar

#Problema 8: Criar as postagens e formatar os posts com css
Solução: Dentro da div área de postagens, criei outra div para servir de primeiro post, nessa div eu configurei as coisas que deveriam ser postadas.
-Foi necessário criar uma nova classe .postagem para realizar as devidas formatações, padding, margin, bgcolor para personalizar os espaçamentos e cores
-Utilizar a tag width na imagem para diminuir seu tamanho em relação ao layout e dar espaçamento
-Tive que dar um padding na área principal para poder separar as postagens do cabeçalho que estava colado, o padding deve ser posto na área principal, não na área de postagens, visto que a área principal engloba tanto as postagens quato o menu lateral.

#Problema 9: A data da postagem não estava sendo formatada, não recebia padding nem margin nem nada.
Solução: Estava acontecendo por causa da tag span que foi utilizada nela, para resolver tive que mudar o DISPLAY para BLOCK

#Problema 10: Os links das postagens estavam pegando a mesma formatação que foi utilizada no cabeçalho
Solução: Para conseguir resolver isso é necessário criar um seletor específico, para que a formatação fique regida apenas para uma área selecionada, não para o documento todo, devemos utilizar a tag id desejada antes de fazer as formatações. 
Ex: #cabecalho a:link, #cabecalho a:visited{}
-Depois de utilizar essa formatação específica, eu defini formatação padrão para todos os links que forem aparecer no documento