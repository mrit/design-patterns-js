<div align="center"><img src="https://lh4.googleusercontent.com/-8weNJa-J78s/VdYZIo8v1gI/AAAAAAAAEq0/qMV4NjREN_Q/w360-h300-no/2015-08-20.png"></div>

Olá pessoal tenho o prazer de apresentar para vocês o começo de uma série de artigos sobre Design Patterns em JavaScript.

## Definição

O que é isso? Porque usar?

Design Patterns ou Padrões de projetos são padrões que descrevem problemas que ocorrem frequentemente e então descreve uma solução ao problema, a fim de poder reusar essa solução milhares de vezes. 

Ok, mas no que isso me ajuda?

Ajuda atribuindo responsabilidade a objetos, deixando o projeto fácil de compreender, reusar e dar manutenção. E claro dando flexibilidade ao mesmo.

Legal mas quando eu vou usar esses padrões?

Você chegou onde eu queria, como é a estrutura de um padrão? Basicamente ele tem quatro elementos essenciais são eles:

>+ Nome
+ Descrição do problema ou contexto para os quais o padrão se aplica
+ Descrição da solução genérica proposta
+ Descrição da aplicação do padrão (custos e beneficios)


Pois bem, o entendimento de como funciona um padrão de projeto pode nos oferecer uma série de benefícios úteis, como por exemplo um raciocínio mais apreciado sobre determinado problema, saber se a solução proposta é ou não um padrão de projeto e até mesmo rever se o padrão utilizado é mesmo necessário ser utilizado.

> Escrever padrões de projetos é uma tarefa desafiadora. Padrões não precisam somente de uma quantidade substancial de material para usuários finais, mas também de uma defesa convicente do porque eles são necessários

Depois de sabermos a definição do que é um padrão de projeto, as vezes pensamos que isso é o suficiente para indentificarmos padrões. Mas não nos enganemos, nem sempre um pedaço de código que estamos olhando está usando um padrão, as vezes ele apenas se parece com um padrão.

Quando olhamos um trecho de código que achamos estar usando algum padrão, devemos listar alguns aspectos do código em que acreditamos que não se trata de um padrão ou conjunto de padrões. Em muitos casos de análise olhamos apenas se o código segue boas práticas e princípios de design que podem coincidir com alguns padrões por acidente. Mas o fato é: `qualquer solução que não faça interações e nem tenha regras definidas, essas soluções não tem padrões`


## Anti-Patterns

Se nós consideramos que padrões são uma boa prática, obviamente anti-patterns representa uma má pratica. Isto é descreve uma má solução para um problema particular que desencadou um mal comportamento.

Alguns exemplos de anti-patterns em JavaScript são:

> + Poluir o contexto global de nossa aplicação com um monte de váriaveis globais
+ Modificar o prototype da classe `Object` ([Este é particulamente um dos mais famosos](http://stackoverflow.com/questions/14034180/why-is-extending-native-objects-a-bad-practice))
 
## Categorias de Design Patterns

Os padrões de projeto são dividos em dois parâmetros: `propósito (criacional, estrutural, compotamental) e escopo  (classes e objetos)`

![categorias design patters](http://www.devmedia.com.br/imagens/articles/226729/Classificacao%20gof.jpg)

#### Propósito
> + Criacional : Processo de criação de objetos
+ Estrutural  : Composição de classes e objetos
+ Comportamental : Interação e distribuição de responsabilidades entre objetos e classes
 
#### Escopo
> + Classe: Relação entre classes e subclasses (herança)
+ Objetos: Relação entre objetos (associação, composição)

## Uma breve introdução a Classes 

JavaScript não tem classes, no entanto elas são simuladas usando funções.

A maneira mais comum de fazer isso é definir uma `function` e depois instanciar com o operador `new`. Nós podemos usar o this para definir novas propriedades e métodos como no exemplo abaixo:

```javascript
// A Racionais "class"
function RacionaisMCs( music ) {
 
  this.music = music;
  this.year = "2014";
 
  this.getInfo = function () {
    return this.model + " " + this.year;
  };
 
}
```

Agora podemos instância um objeto usando a função construtora `RacionaisMCs` que acabamos de definir:

```javascript
var musicaPreferida = new RacionaisMCs("Negro Drama");

musicaPreferida.year = "2002";

console.log(musicaPreferida.getInfo());
```

Para mais maneiras de definir classes, olhe este [link](http://www.phpied.com/3-ways-to-define-a-javascript-class/)
