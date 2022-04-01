Aqui deixarei registrados as dificuldades e observações encontradas na criação do projeto e como é a solução, caso seja encontrada

---DICAS---
*Poderia ter feito uma tag div para todo o conteúdo já na largura de 900px, desse modo não precisaria colocar individualmente cada medida nas tags externas.
*A tag padding também produz um espaçamento, sem necessitar da tag br para dar espaço

#PROBLEMA 1: Deixar as bordas da caixa no mesmo tamanho da imagem no cabeçalho.
Solução: Para isso, bastou utilizar a tag width no css externo .borda, setando o valor de 900 pixels foi possível chegar na largura exata da imagem. (OBS, o mesmo poderia ter sido feito com a altura (height), cuja a qual no início coloquei br para chegar na altura desejada.)

#PROBLEMA 2: Links do cabeçalho estavam muito próximos um do outro, não deixando um espaçamento
Solução: Usar o padding para espaçamento

#PROBLEMA 3: Criar uma caixa de envio de contato, ao clicar em enviar não acontecia nada
Solução: Para isso, é necessário que os inputs estejam dentro de uma tag form, então é só criar a mesma
