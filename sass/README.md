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

```scss
@import "colors.scss"

@import "typography.scss"

Partials

@import "_layout.scss"

@import "_buttons.scss"
```



### VARIÁVEIS

1. Criação de variáveis para cores, componentes e etc
2. Ajuda na organização e consistência no design
3. Também pode ser utilizado para propriedades CSS

exemplo:

```scss
$preto: #000;

$branco: #FFF;

$gray1: #111;

$gray2: #555;

$box-shadow: blue;
```



### ANINHAMENTO OU NESTING

1. Criação de efeitos cascata do CSS com mais facilidade
2. Pode emendar n cascatas
3. Facilita na identificação de qual elemento está estilizando
3. Nesting de tags e propriedades

exemplo:

```scss
ul {

​	li {

​		list-style: none;

​		a {

​		text-decoration: none;		

​		}

​	}	

}
```



### @mixin & @content

Podemos usar padrões no código, declarando somente uma vez e utilizando o @include.

1. Criação de funções pré-definidas
2. Aproveitamento de código
3. Criação de sistemas mais completos
4. Facilidade para adicionar prefixos
5. Facilita na criação de função de responsividade.

exemplo:

```
@mixin nome_mixin($cor: #FAFAFA){ 

​	font-size: 36px;

​	color: $cor;

​	@content;

}
h1 {
	@include nome_mixin(#FFF) {
		line-height: 110%;
	}
}
```

### @if & @else e Operadores

Podemos utilizar o @if & @else junto com @mixins, como exemplo na aplicação na responsividade.

1. Criação de estruturas encadeadas
2. Dá mais elasticidade aos @mixins
3. Capacidade de criar cenários diferentes de estilização

exemplo:

	@if $layout == light {
	 	$bg-color: #EFEFEF;
	 	$text-color: #101010;
	}
	
	@else if $layout == dark {
		$bg-color: #101010;
		$text-color: #EFEFEF;
	}

### Estruturas de Repetição: @for, @while e @each

Sequências de códigos que estabelece como um loop deve se repetir ~ basicamente.

1. Criação de estruturas de repetição
2. Dá mais possibilidades aos @mixins & @functions

exemplo:

```scss
@for $i from 1 through 12 {
	.grid-#{$i} {
		width: 72px * $i
	}
}
.grid-1 {
    width: 72px;
}

.grid-2 {
    width: 144px;
}
```

@for => você estabelece um vetor, ele já vai rodar automaticamente dentro do parametro.

@while => consegue colocar algumas comparações, diferente do @for

