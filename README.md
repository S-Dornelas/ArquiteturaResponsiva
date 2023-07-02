# Arquitetura Responsiva

Com este projeto consegui aprender e construir um site responsivo.

Adotei o Atomic Design que consiste na ideia de criar um arquivo CSS para cada elemento da página, basicamente é um modelo de organizar os componentes, pastas e a estrutura do nosso CSS a partir do princípio de átomos, onde um átomo é toda tag HTML. Juntos esses elementos, ou átomos, formam uma "molécula" - nesse caso, a molécula de um formulário de pesquisa.

A junção de várias moléculas, por sua vez, forma os "organismos". Por exemplo, juntando a molécula referente ao formulário de pesquisa com a molécula referente ao menu (que também tem seus átomos, como a imagem e os links), temos um organismo que representa o cabeçalho de uma página.

Unindo vários organismos, chegamos aos "templates". No exemplo, temos o organismo referente ao cabeçalho, ao banner e à descrição, e que juntos formam um template.

Por fim, o template dá lugar a uma página.

A diferença básica entre um template e uma página é que os templates são feitos com informações não reais, como um Lorem Ipsum (texto padrão em latim utilizado para testar fontes e diagramação), imagens vazias no lugar dos logos e banners, e assim por diante. Nas páginas, utilizamos imagens e informações reais do nosso protótipo.

De volta ao projeto, vemos que as tags `<header>`, `<img>`, `<nav>` e `<ul>` são todas átomos; a junção dos átomos `<nav>` e seus filhos (`<ul>` e `<lu>`) forma uma molécula; e a junção dessa molécula com outros átomos e moléculas define o organismo "cabeçalho". Com isso, conseguiremos simplificar bastante a manutenção e evolução do nosso projeto, podendo simplesmente criar novas pastas e/ou arquivos para adicionarmos novos componentes.

Devemos seguir basicamente essa regra: se o componente é composto por apenas um arquivo, ele pode ser criado na própria raiz da pasta "css"; do contrário, se for composto por vários arquivos, deveremos criar uma nova pasta para comportá-los.
