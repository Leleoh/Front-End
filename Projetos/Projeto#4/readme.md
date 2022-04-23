Aqui deixarei registrados as dificuldades e observações encontradas na criação do projeto e como é a solução, caso seja encontrada

---Dicas---
*Fazer o fundo com a tag background no estilo css externo ao invés de inserir diretamente no html (avaliar o caso)
*Sempre ir montando a estrutura do site com elementos testes, background coloridos, textos, etc, pra ver se ta alinhando mesmo e ter perspectiva do que ta fazendo

#Problema 1: Criar o cabeçalho no devido tamanho, centralizado. Solução: Usar divs e formatar o tamanho no css externo

#Problema 2: A imagem auxiliar do cabeçalho estava entrando na área da barra de navegação e estava fora do tamanho desejado. Solução: Aparentemente estava havendo um conflito entre um margin de uma class e um padding de uma id, o margin acabava jogando toda a "box" para baixo, então o plano de fundo (brasilzinho) se movia junto para baixo e invadia os outros espaço.

#Problema 3: Criar uma barra de navegação horizontal no cabeçalho. Solução: Criar uma UL contendo Li's para gerar uma lista sem ordem, preencher a lista com links e depois formatar esses links. Nesse momento, formatei somente a ul que se encontra dento do id #topo, pois podem existir outras uls ao longo do código, usei a tag float para tirar uma de baixo da outra e colocar lado a lado.

#Problema 4: Criar as colunas com seus respectivos conteúdos, e dessa forma conseguir separá-las, e dar espaçamento entre o cabeçalho e o conteúdo. Solução: Criar novas divs com margin top para descer até a área desejada, depois formatar no css externo para ajustar tamanho, posição e propriedades

#Problema 5: Ajustar as caixas de conteúdo, onde ficarão imagens, categorias, recentes, etc. Solução: Criar classes e ids para serem formatados ao bel prazer no css externo


