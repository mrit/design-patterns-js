![Design Patterns] (http://www.dev-metal.com/wp-content/uploads/2014/06/javascript-design-patterns-cover-1.jpg)

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

Se nós consideramos que padrões são uma boa prática, obviamente anti-patterns representa uma má pratica, sendo mais prático seria uma um problema que já aprendemos a lidar pois agora temos um padrão para que consegue resolvê-la.

Alguns exemplos de anti-patterns em JavaScript são:

> + Poluir o contexto global de nossa aplicação com um monte de váriaveis globais
+ Modificar o prototype da classe `Object` ([Este é particulamente um dos mais famosos anti-patterns](http://stackoverflow.com/questions/14034180/why-is-extending-native-objects-a-bad-practice))
 
