<h1 align="center">C++ Essentials</h1>

<h2 align="center">Por Fabio Carneiro</h2>



## Prefácio

**E**ste livro poderá sofrer alterações no futuro, e é de suma importância que o leitor crie o hábito de lê-o com uma certa frequência, será escrito à medida que me for cabível de tempo, e disposição, irei condensar neste material tudo o que eu pude usar em busca de conhecimento, seja por livros, blogs, fóruns, cursos, experiências próprias, absolutamente toda via de aprendizado que eu obtive e ainda vou obter, vou transcrever aqui em forma de conhecimento escrito e facilitado, **C++ Essentials** tem o objetivo de fornecer todo conhecimento **essencial** que um desenvolvedor C++ precisa, e o que não for abordado neste livro, será abordado no [repositório do projeto](https://github.com/bynmboy/linguagemcpp).

**E**ste Livro será dividido em capítulos, com assuntos condizentes com a fase de aprendizado, para que tudo seja um aprendizado continuo e linear, suave, e de modo que mesmo que não consiga por em práticas os exercícios ou exemplos do livro, ainda assim sua leitura seja o suficiente para seu aprendizado de modo que, seja possível que alguns termos ou nomes técnicos estejam diferentes dos comumente encontrados para que seu entendimento seja mais facilitado. Eu defendo a ideia de que, um tema que não seja primeiro entendido, não possa ser posto em prática, e se não há prática de um tema entendido, não há aprendizado pensando por este caminho, será pensado e arquitetado para que em primeiro ponto seja de fácil entendimento, para que suas práticas tenham sentido e seu conhecimento de fato, ocorra.



## Autor

**M**eu nome é Fabio Carneiro, conheci a tecnologia cedo, meu primeiro contato programação foi com um Commodore 64 de um colega de sala quando eu tinha meus 12 anos, a gente saía da sala, ia para a casa dele e passávamos algumas horas copiando códigos da linguagem Basic de uma revista em inglês que mal sabíamos o que estavam escritos nas páginas, mas olhando as figuras logo entendíamos do que se tratava, e confesso que eram poucas as vezes que conseguíamos rodar um jogo, mesmo depois de horas de escritas e revezamento, anos depois, mais precisamente 1 ano e meio depois, eu me inscrevi em um projeto da minha cidade onde preparava os jovens para iniciar sua carreira como jovem aprendiz, em um projeto social que o governo havia implementado na Cidade, me inscrevi em um curso onde aprendíamos usar o sistema GNU/Linux Ubuntu, chuto que usávamos a versão 10.04, nesta época eu já possuía um computador em casa que minha Mãe sofreu muito para poder pagar, um incrível Celeron mono-núcleo com 256MB de memória RAM, uma capacidade de armazenamento de 40GB, nesta época não só conheci sistemas Linux como conheci minha paixão, o Slackware.

**P**edi uma cópia do CD-Rom para o professor do curso, e infelizmente ele não tinha, mas na aula da semana seguinte ele me trouxe um CD e disse que se eu dominasse aquele sistema, eu com certeza seria um aluno diferenciado, e o mesmo me custou meses para somente instalar o sistema em um hd de 20GB que adquiri juntando latinhas de refrigerantes e trocando com uma mulher que as recolhiam e te pagava por quilo do alumínio, mas no caso vi o hd e arrisquei e paguei o preço da sucata.

**A**lgum tempo depois me inscrevi em outro projeto social do governo que nos preparava para o mercado de trabalho, nesta época eu já tinha 14 anos de idade e neste projeto fiz um curso de informática patrocinado pela Intel, onde aprendi conceitos básico da linguagem C, linguagem Pascal e HTML 4. Depois disso com 16 fui trabalhar com indústria, pensei que jamais iria ver códigos de programação. meses depois em um sábado fui operar uma máquina C.N.C, Comandos Numéricos Computadorizados, que me fez me reaproximar dos códigos. Pelas dificuldades que enfrentei, me afastei dos estudos e voltei a estudar em 2014, em 2021 iniciei a faculdade de Engenharia de Software pela Universidade Anhanguera Educacional.

**A**tualmente acumulo mais de 50 cursos concluídos divididos em diversos temas das áreas de desenvolvimento de softwares e linguagens de programação. Acumulei ao longo de 18 anos conhecimento no Universo Linux em diferentes bases de distribuição, estou cursando Faculdade de Engenharia de Software, me especializando em desenvolvimento de sistemas comerciais para web, computação gráfica, análise e desenvolvimento de sistemas, arquitetura de software entre outros sub-gêneros condizentes com meu plano de carreira.


## O Básico de C++



**O** Básico que precisa saber sobre a linguagem é que ela une muitos elementos interessantes, como Desempenho, versatilidade, estrutura bem definida e muitas, muitas possibilidades de ser cabível de ser utilizada em literalmente quase tudo que se possa imaginar, com uma pesquisa minuciosa na internet, você descobrirá que existem recursos, projetos entre outros que te possibilita usar C++ para desenvolvimentos web, desktop, mobile, games, engenharia e muito mais.

**A** Linguagem C++ não é uma linguagem difícil, mas em muitos pontos pode ser confusa, muitas pessoas pelas comunidades, grupos, se vangloriam dizendo que C++ é para quem é sobre-humano, mas não caia nessa, não somente C++ como toda e qualquer linguagem é para quem tem vontade de aprender e estudar, e lembre-se, a dificuldade de aprender algo não esta ligado ao que está aprendendo e sim à quem está aprendendo, uma pessoa pode ter facilidade com Java e dificuldade com C++ e uma outra pessoa pode ter o efeito contrário, apenas siga em frente.

**T**ambém podemos ver coisas incríveis feitas com C++ como por exemplo sistemas operacionais, como no caso do [Haiku-OS](https://www.haiku-os.org/) e muitas outras coisas mais



## Começando com C++



**O** que você precisa saber antes de começarmos é que C++ é uma linguagem multiparadigmática e de multipropósito, podendo assim ser usada com os paradigmas de OOP (Orientação à Objetos), Procedural e genérica, é uma linguagem de nível de sistema que fornece abstrações de alto nível com baixíssimo tempo de execução e custos de desenvolvimento quando montado um ambiente minimalista, mas também existindo IDE com um porte muito maior com ferramentas profissionais de excelente qualidade para desenvolvimentos corporativos para empresas de grande porte ao redor do mundo.

**A** Linguagem é humanamente legível, ou seja, é ler e entender do que se trata, mas em alguns momentos, haverá "gramáticas" que te confundirá necessitando de pesquisas e paciência, no demais, vamos ver um código e vamos para análise.



> Obs. Você pode usar diversos tipos diferentes de editores de texto, compiladores, e não vou abordar isso aqui porque o foco é a linguagem em si, como você vais estudar os códigos, seja um editor gráfico, ou cli, seja VSCODE ou Geany, isso é cabível de sua escolha, não tenho o poder de saber o que irá usar, logo focarei na linguagem.



```c++
#include <iostream> // 1

int main (int argc, char *argv[]) //2
{ // 3
    std::cout << "Aprendendo C++" << std::endl; // 4
    system("PAUSE"); // 5
    return 0; // 6
} // 3.1
```



**O** código no quadro acima é um programa completo no mais simples que poderia fazer, e ainda assim contem elementos interessantes, antes de ficar confuso eu fiz comentários seguidos de um número ex:

``` c++
// 1
// 2
// 3 ...
```

**E**stas "coisas" chamamos de comentários. Os comentários são ignorados pelo compilador, ele apenas serve para fazer anotações que empregam um propósito que você definir, como um lembrete caso você fique algum tempo sem trabalhar no projeto, ou um comentário de coisas para fazer como uma lista de "TODO" enfim, o que precisa saber é que para o compilador ele será ignorado, e eu usei o comentário para mostrar para você itens isolados do nosso código para explicar para você o que é cada um deles.

**N**o comentário "//1" é a nossa primeira linha de programa, é uma diretriz de compilação, vai ler por aí que essa instrução, e entenda instrução como um comando que você está ordenando ao seu programa, que neste caso chamados de diretriz de compilação porque o comando basicamente está representando o seguinte:

> Compilador, este programa usa recursos que para funcionar você precisa usar a biblioteca "iostream" então inclua ela na hora de compilar meu programa.

**O**u seja, é um aviso para o compilador do que ele precisa incluir ao nosso programa quando ele for compilar, e *iostream* é uma biblioteca que chamamos de padrão, por que não precisamos informar em nada na hora de compilar o nosso programa, apenas mandamos compilar e o compilador dará conta do recado, muitas bibliotecas, no momento em que vamos compilar o programa, no caso de compilar manualmente pelo terminal, precisamos informar para o compilador usando argumentos, mas não vou me aprofundar neste momento, na hora certa deixarei alguns exemplos para esclarecer melhor isso. Esta biblioteca " iostream " é responsável por fornecer ao nosso programa recursos de entrada e saída de dados, ou seja, com ela, podemos digitar algo e será lido pelo nosso programa, tal que se mandarmos nosso programa mostra algo no terminal, isso será uma saída de dados, em outro momento eu coloco um exemplo onde vamos ter uma entrada de dados para exemplo, neste primeiro usamos apenas a saída de dados.

**N**o comentário " // 2 " temos o item mais importante do nosso programa, o chamado "Método Main" ele é o responsável por dizer ao programa, onde é o inicio de tudo, sem ele o programa simplesmente não funciona, nessa linha temos o cabeçalho de uma função, e uma função em programação é um "microcódigo" que dentro dele temos um "programinha" com instruções, dados e muito mais, nesta linha podemos dividir em partes para facilitar seu entendimento da seguinte forma:

```c++
int		//	->		tipo de dado de retorno da função (ainda vai aprender o que é retorno). 
main	//	->		nome que a função terá e por qual nome ela será reconhecida no sistema todo. 
(		//	->		abertura da sessão de parâmetros da função, ou seja informações ou dados que ela precisa ou não receber.
int 	//	->		tipo de dado do primeiro parâmetro.
argc	//	->		nome do primeiro parâmetro.
,		//	->		a virgula aqui, representa que vamos ter um outro parâmetro, caso seja só um, não precisa ter ela.
char	//	->		tipo de dado do segundo parâmetro.
*		//	->		esse sinal representa um "ponteiro" ainda vai aprender sobre isso.
argv	//	->		nome do segundo parâmetro.
[]		//	->		isso representa um vetor, ainda vai aprender o que é vetor mas aqui dizemos que temos um vetor.
)		//	->		fechamento da sessão de parâmetros da função main.
```

**N**o comentário " // 3 " temos temos a abertura do escopo da nossa função, entenda escopo como um espaço, um limite ou uma área, quando definirmos uma função, precisamos dizer onde ela começa e onde ela termina, para que o compilador saiba o que pertence ao escopo daquela função, se observar na ultima linha temos o comentário " // 3.1 " que representa o fechamento do escopo da função main.

**N**o comentário " // 4 " temos então a nossa primeira instrução e o que o nosso programa fará. vamos desmembrar esta linha para que fique fácil seu entendimento:

```c++
std		//	->	std é um namespace, um indicativo que ele faz parte de um "grupo" de "coisas".
::		//	->	esse sinal representa que o que está a direita dele, pertence ao que está a esquerda dele "cout pertence à std".
cout	//	->	esse por sua vez é o comando de saída de dados que pertence ao "namespace" que ainda vai aprender, de nome std.
<<		//	->	esse sinal é "deslocamento de bits à esquerda" e neste caso estamos fazendo uma sobreposição do operador para fluxo de saída, para dizer que o que está a direita será deslocado para à esquerda, e nesse caso, o que vem a sua direia será direcionado para "cout", direcionado para a saída.
"Aprendendo C++"  //  ->  aqui temos uma "String" quando eu falar de tipos de dados entenderá melhor, mas é uma cadeia de letras ou cadeia de caracteres, usamos para passar valores alfanuméricos.
<<		//	->	deslocamento de bits à esquerda como citei anteriormente.
std		//	->	namespace std que foi explicado seu uso.
::		//	->  operador de "resolução de escopo" também explicado seu uso.
endl	//	->  esse cara é um "quebra-linha" ele diz onde uma linha acaba para se iniciar uma nova linha, mas esse em específico vai além, não só quebra ou termina a linha como ele faz o descarregamento de buffer, ele limpa o buffer se houver algo, mais pra frente aprenderá melhor sobre isso. 
;		//	->	aqui definimos onde uma instrução termina, no caso da função main, ela termina com } e não precisa de ; para finalizar, mas quando temos uma instrução ou "uma linha de código" usamos o sinal de "ponto e virgula" para finalizar ela, sem o sinal colocado no final, seu programa dará erro e não irá compilar.
```

**N**o comentário " // 5 " temos uma instrução que só surtira efeitos em alguns casos e somente no sistema Windows, como por exemplo executar um programa pelo Visual Studio Community, quando mandar compilar e executar seu programa, uma janela de terminal se abrirá tão rápido que não conseguirá ver o que aconteceu, então utilizamos esta instrução para que o terminal fique aguardando você digitar algo para que ele feche, te permitindo ver o que seu programa mostrou no terminal antes de fechar, em caso de usar diretamente o terminal, esteja você utilizando um sistema Linux, Windows ou qualquer outro, essa instrução não terá utilidade.

**N**o comentário " // 6 " temos uma instrução que claramente diz que o programa retorna 0 (zero) como disse anteriormente nossa função main tem um tipo, assim como os parâmetros que ela recebe também, no caso da main temos:

> int main ...

**O**u seja, ela é do tipo *int* que representa *integer* ou se preferir *inteiro* então como está função é o coração do nosso programa, ela precisa informar ao sistema operacional o que está havendo, por exemplo, como saber se o programa foi executado com sucesso ou se houve um erro ? Neste caso a instrução:

> return 0;

**E**stá dizendo que o programa executou e foi um sucesso! Podemos retornar qualquer valor inteiro, mas para nesse caso o programa tem que iniciar e terminar, e como queremos que ele termine com sucesso em sua tarefa, dizemos que a função main retorna 0 que representa exatamente isso. Obviamente há muitas dúvidas quanto a tudo que vimos até aqui, mas com o tempo, leitura, estudo e prática sanará todas elas.







<h3 align="center">Quer apoiar o projeto e meu trabalho? Faça um pix para a chave:<h3>

<h4 align="center">fabioaacarneiro@gmail.com</h4>

<h4 align="center">NuBank, Fabio Aparecido Affonso Carneiro</h4>

<h4 align="center">A sua ajuda colaborará para a continuação deste livro e para realização de projetos futuros!</h4>

<br>
    <p align="center"><a href="https://github.com/bynmboy/linguagemcpp">Início<a></p>
<br>

<p  align="center"><img src="https://github.com/bynmboy/linguagemcpp/blob/main/logo-c%2B%2B.png" width="200" height="200"/></p>
