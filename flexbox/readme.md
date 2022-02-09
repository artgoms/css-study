// Flex - Container

display: flex
Define o elemento como um flex container, tornando os seus filhos flex-items

// flex-direction
Define a direção dos flex-items. Por padrão ele é row(linha), por isso quando o display:flex é adicionado, os elementos ficam em linha, um do lado do outro.

/ flex-direction: row;
/ flex-direction: row-reverse;
/ flex-direction: column;
/ flex-direction: column-reverse;

// flex-wrap
Define se os itens devem quebrar ou não a linha. Por padrão não quebram linha, isso faz com que os flex-itens sejam compactados além do limite do conteúdo.

/ flex-wrap: nowrap;
Valor padrão, não permite a quebra de linha.

/ flex-wrap: wrap;
Quebra a linha assim que um dos flex items não puder ser mais compactado.

/ flex-wrap: wrap-reverse;
Quebra a linha assim que um dos flex items não puder manter compactado. A quebra é na direção contrária, ou seja, para a linha acima.

// flex-flow
É um atalho para as propriedades flex-direction e flex-wrap. Você não verá muito o seu uso, pois geralmente quando mudamos o flex-direction para column, mantemos o padrão do flex-wrap que é nowrap.

/flex-flow: row nowrap;
Coloca o conteúdo em linha e não permite a quebra de linha.

/flex-flow: row wrap;
Coloca o conteúdo em linha e permite a quebra de linha.

/flex-flow: column nowrap;
Coloca o conteúdo em coluna e não permite a quebra de linha.

justify-content

align-items

align-content

// Flex - Item

flex-grow

flex-basis

flex-shrink

flex

order

align-self
