Aqui deixarei registrados as dificuldades e observações encontradas na criação do projeto e como é a solução, caso seja encontrada

---Dicas---
*Fazer o fundo com a tag background no estilo css externo ao invés de inserir diretamente no html (avaliar o caso)

*Sempre ir montando a estrutura do site com elementos testes, background coloridos, textos, etc, pra ver se ta alinhando mesmo e ter perspectiva do que ta fazendo

*Aplique primeiro formatações padrão e depois caso necessário utilize classes para alterá-las especificamente

----------------------------------------------------------------------

#Problema 1: Criar o cabeçalho no devido tamanho, centralizado. Solução: Usar divs e formatar o tamanho no css externo

#Problema 2: A imagem auxiliar do cabeçalho estava entrando na área da barra de navegação e estava fora do tamanho desejado. Solução: Aparentemente estava havendo um conflito entre um margin de uma class e um padding de uma id, o margin acabava jogando toda a "box" para baixo, então o plano de fundo (brasilzinho) se movia junto para baixo e invadia os outros espaço.

#Problema 3: Criar uma barra de navegação horizontal no cabeçalho. Solução: Criar uma UL contendo Li's para gerar uma lista sem ordem, preencher a lista com links e depois formatar esses links. Nesse momento, formatei somente a ul que se encontra dento do id #topo, pois podem existir outras uls ao longo do código, usei a tag float para tirar uma de baixo da outra e colocar lado a lado.

#Problema 4: Criar as colunas com seus respectivos conteúdos, e dessa forma conseguir separá-las, e dar espaçamento entre o cabeçalho e o conteúdo. Solução: Criar novas divs com margin top para descer até a área desejada, depois formatar no css externo para ajustar tamanho, posição e propriedades

#Problema 5: Ajustar as caixas de conteúdo, onde ficarão imagens, categorias, recentes, etc. Solução: Criar classes e ids para serem formatados ao bel prazer no css externo

#Problema 6: Colocar as caixas nos devidos lugares, por exemplo, a área lateral estava na direita, sendo que seu lugar é na esquerda. Solução: Usar o margin para organizar as posições, usando margin negativo e positivo

#Problema 7: Em algumas páginas não terão três colunas de informações e conteúdos, podendo variar para duas ou até mesmo uma. Solução: Criar um id "três-colunas" e "duas-colunas" no body, e adaptar para as páginas que não irão possuir três colunas posteriormente, avaliando cada caso, mudar então o tamanho "width" ocupado por cada elemento daí.

#Problema 8: Configurar a barra lateral com o hover e a imagem para dar o efeito, no momento em que o hover é aplicado a imagem sai em cima do texto. Solução: Criar uma seleção especifica de id onde o <a> está contido, então aplicar a propriedade hover, depois nessa propriedade aplicar color, bg-color, e um padding left, para tirar a imagem de cima do texto.

#Problema 9: Colocar a imagem no tamanho certo. Solução: O ideal seria trabalhar com a imagem editada no tamanho correto, mas como não é o caso, deve-se fazer um redimensionamento width em 100%, desse modo ocupando toda a área disponível da coluna.

#Problema 10: Colocar uma borda cinza na imagem. Solução: Foi só criar uma nova formatação no css externo marcando a img.


