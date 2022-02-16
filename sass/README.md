# SASS

### O que é o SASS?

É um pré-processador de CSS. Melhora a performance na programação CSS. Adiciona variáveis, funções, etc;

O SASS dá um boost no CSS com skills de linguagem de programação, mas não faz nada além do que o CSS puro não faça.



### Vantagens

Declaração de funções

Variáveis

Facilidades com pseudo-elements e estados

Melhora a compatibilidade dos browsers



#### SASS vs SCSS

O SASS se distância muito devido ao fato de ter sido muito simplificada, condicionando o cérebro a um sintaxe do css padrão.

Já o SCSS nos deixa numa sintaxe perto do padrão do CSS, não condicionando ao esquecimento do padrão.



## Fundamentos do SASS

### @import

1. Quando é possível importar arquivos SASS em outros para copilar em um só.
2. Melhora a organização. Conceito de componentes!
3. Otimiza as requests: o site fica mais otimizado com menos arquivos para carregar.
4. **A ordem importa!**
5. Uso de partials: _arquivo.scss - melhora e faz com que copile em um só arquivo, não criando "arquivo.css.map", por exemplo.

exemplo:

@import "colors.scss"

@import "typography.scss"

Partials

@import "_layout.scss"

@import "_buttons.scss"



### VARIÁVEIS

1. Criação de variáveis para cores, componentes e etc
2. Ajuda na organização e consistência no design
3. Também pode ser utilizado para propriedades CSS

exemplo:

$preto: #000;

$branco: #FFF;

$gray1: #111;

$gray2: #555;

$box-shadow: blue;



### ANINHAMENTO OU NESTING

1. Criação de efeitos cascata do CSS com mais facilidade
2. Pode emendar n cascatas
3. Facilita na identificação de qual elemento está estilizando
3. Nesting de tags e propriedades

exemplo:

`ul {`

​	`li {`

​		`list-style: none;`

​		`a {`

​		`text-decoration: none;`		

​		`}`

​	`}`	

`}`
