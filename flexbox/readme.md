# Flex - Container

display: flex
Define o elemento como um flex container, tornando os seus filhos flex-items

#### flex-direction

Define a direção dos flex-items. Por padrão ele é row(linha), por isso quando o display:flex é adicionado, os elementos ficam em linha, um do lado do outro.

/ flex-direction: row;
/ flex-direction: row-reverse;
/ flex-direction: column;
/ flex-direction: column-reverse;

#### flex-wrap

Define se os itens devem quebrar ou não a linha. Por padrão não quebram linha, isso faz com que os flex-itens sejam compactados além do limite do conteúdo.

/ flex-wrap: nowrap;
Valor padrão, não permite a quebra de linha.

/ flex-wrap: wrap;
Quebra a linha assim que um dos flex items não puder ser mais compactado.

/ flex-wrap: wrap-reverse;
Quebra a linha assim que um dos flex items não puder manter compactado. A quebra é na direção contrária, ou seja, para a linha acima.

#### flex-flow

É um atalho para as propriedades flex-direction e flex-wrap. Você não verá muito o seu uso, pois geralmente quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é nowrap.

/flex-flow: row nowrap;
Coloca o conteúdo em linha e não permite a quebra de linha.

/flex-flow: row wrap;
Coloca o conteúdo em linha e permite a quebra de linha.

/flex-flow: column nowrap;
Coloca o conteúdo em coluna e não permite a quebra de linha.

#### justify-content

Alinha os itens flex no container de acordo com a direção. A propriedade só funciona se os itens atuais não ocuparem todo o container.

###### justify-content: flex-start;

Alinha os itens ao início do container.

###### justify-content: flex-end;

Alinha os itens ao final do container.

###### justify-content: center;

Alinha os itens ao centro do container.

###### justify-content: space-between;

Cria um espaçamento igual entre os elementos. Mantendo o primeiro grudado no inicio e o último no final.

###### justify-content: space-around;

Cria um espaçamento entre os elementos. Os espaçamentos do meio são duas vezes maiores que o inicial e final.

### align-items

Alinha os flex items de acordo com o eixo do container. O alinhamento é diferente para quando os itens estão em colunas ou linhas.

###### align-items: stretch;

Valor padrão, ele que faz com que os flex itens cresçam igualmente

###### align-items: flex-start;

Alinha os itens ao inicio.

###### align-items: flex-end;

Alinha os itens ao final

###### align-items: center;

Alinha os itens ao centro

###### align-items: baseline;

Alinha de acordo com o conteúdo.

### align-content

// Flex - Item

flex-grow

flex-basis

flex-shrink

flex

order

align-self
