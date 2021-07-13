# Preparando o ambiente para Programar em C++ no Windows 

## Instalando o compilador G++

* Acesse o site baixo para instalar o g++ para Windows:
  * https://jmeubank.github.io/tdm-gcc/articles/2021-05/10.3.0-release

No link acima será possível desfrutar das opções de downloads para que possamos ter em nosso computador o compilador, que é responsável por transformar nossos códigos C++ em um binário executável capaz de reproduzir nosso programa ...

![Alt text](https://github.com/bynmboy/gcc-windows-guide/blob/main/img/tdmgcc.PNG)

Como podemos analisar na imagem logo acima deste texto que está lendo neste momento, está claro que podemos desfrutar de 3 opções de downloads que são eles, de cima para baixo: *"tdm-gcc-webdl.exe"* que é uma opção minimalista do instalador do compilador que vai te permitir selecionar os componentes que você deseja, baixá-los e por fim, instá-los em sua máquina, em sequência temos a segunda opção *"tdm64-gcc-10.3.0-2.exe"* esta é uma opção onde baixamos um instalador mais completo, que nos permite compilarmos programas não somente para arquitetura 32bits como para 64bits também, por estar marcado, já fica nítido que será ele que vamos usar, mas vamos seguir o ritmo e e compreender a terceira opção de download, diferentemente da opção que marcamos na imagem, esta terceira opção será usada caso o seu computador esteja usando um sistema operacional Windows com arquitetura de 32bits.

* Depois de baixado e iniciado a instalação do instalador do compilador, podemos seguir passos simples mas necessários para instalarmos o compilador no computador, como por exemplo clicar no botão *"Create"* por hora, só é necessário saber que ele irá "criar" uma nova instalação, mas para não te deixar curioso e explicando de forma resumida, a opção *"Manage"* te permite remanejar uma instalação já existente em seu computador e *"Remove"* irá remover uma instalação já existente em sua máquina.

  ![Alt text](https://github.com/bynmboy/gcc-windows-guide/blob/main/img/tdm-setup.PNG)

* Agora vamos selecionar qual arquitetura queremos que o nosso compilador use como base para compilar nossos códigos, no meu caso vou margar a opção de baixo que diferente da opção de cima que só compila para 32 bits, ele compilará para 32 e 64bits, e prosseguimos clicando em *"Next >"*

  ![Alt text](https://github.com/bynmboy/gcc-windows-guide/blob/main/img/gccarch.PNG)

* Selecionamos agora onde será instalado o nosso compilador, no meu caso eu precisei procurar o diretório onde já continha à instalação que eu havia feito anteriormente, mas você pode procurar um lugar diferente, em seguida, clicamos outra vez na tecla *"Next >"*

  ![Alt text](https://github.com/bynmboy/gcc-windows-guide/blob/main/img/dirsetup.PNG)

* E agora vamos fazer uma configuração básica do que será instalado junto do nosso compilador, como por exemplo os pacotes, então recomendo que deixe a opção *"TDM-GCC Recommnded, All Packages"* e em seguida no botão *"Install"* para darmos início na instalação propriamente dita.

  ![Alt text](https://github.com/bynmboy/gcc-windows-guide/blob/main/img/instalation.png)

* Concluído a instalação, teremos uma tela como a imagem a seguir, mostrando o *status* de *"Completed successfully"* confirmando que a instalação foi completada com sucesso, e agora, já sabe, clique no botão *"Next >"*

* Finalizado! Agora precisamos clicar em *"Finish"* e como a opção *"Read the TDM-GCC README file (recommended)"* está marcada, ao clicar no botão para finalizar a instalação, será aberto um arquivo do tipo [*Markdown*](https://pt.wikipedia.org/wiki/Markdown) que pode ser aberto e melhor visualizado em programas como [*Typora*](https://typora.io/), este arquivo contém muita coisa sobre o compilador, recomendo muito que leia, caso não entender nada de inglês podemos usar o [google tradutor](https://translate.google.com.br/?hl=pt-BR). E finalizamos nossa instalação do compilador pronto para compilar nossos códigos em programas reais!

* Baixe a IDE, *Integrated Development Environment (*  ***Ambiente de Desenvolvimento Integrado*** ) que no nosso caso sera o [Code::Blocks](https://www.codeblocks.org/) ou se preferir (*ou for preguiçoso*) pode acessar a página contendo as opções de download que é possível desfrutar no site, clicando [aqui](https://www.fosshub.com/Code-Blocks.html?dwl=codeblocks-20.03-setup.exe), como neste guia eu ensino instalar o compilador a parte, eu usei para este exemplo a opção que pode ser baixada clicando [aqui](https://www.fosshub.com/Code-Blocks.html?dwl=codeblocks-20.03-setup.exe) mas pode fique à vontade para escolher uma opção que melhor te atenda.

* Uma vez baixado e iniciado o instalador, estaremos diante de uma imagem similar com a imagem à seguir:

  ![Alt text](https://github.com/bynmboy/gcc-windows-guide/blob/main/img/codeblocks1.png)

  Creio que não é preciso mencionar que vamos clicar em *"Next >"* não é mesmo ?

  * Aceite os termos de contrato e licença clicando em *"I Agree"* :

    ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/codeblocks2.png)

    * Na tela seguinte, podemos escolher quais componentes farão parte da instalação, "geralmente" por padrão já é possível visualizar que será instalado a opção mais completa, nos restando prosseguir clicando em *"Next >"*

      ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/codeblocks3.png)

      * Pois bem, agora vamos precisar mudar caso necessário, o lugar (*diretório*) de onde será instalada nossa IDE Code::Blocks, neste caso, vou precisar apenas clicar em install.

        ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/codeblocks4.png)

        * Finalizado a instalação agora podemos clicar em *"Sim"* e o Code::Blocks será iniciado para nós.

          ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/codeblocks5.png)

          E agora teremos a IDE rodando *bonitamente* como na imagem a seguir:

          ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/codeblocks6.png)

  ## Após instalado os pacotes, podemos iniciar o teste!

  Agora podemos iniciar um novo projeto na IDE code::blocks e assim, iniciarmos um teste prático fazendo o "Hello World".

  

  ```
  #include <iostream>
  
  int main (){
  	std::cout << "Hello World" << std::endl;
  	return 0;
  }
  ```

  ​			

**exemplo**

![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/helloworld.png)



## Então, vamos criar um novo projeto para fazer o exemplo acima:

* criando o projeto:

  ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/newproject.png)

  

* Criamos um projeto vazio:

  ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/empty.png)

  

* Definindo um nome, local para o projeto e depois em Next...

  ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/setname.png)

* No meu caso criei uma nova biblioteca de nome *"Projetos C++"* e criei uma pasta designada a ser o diretório do projeto, chamada *"Projeto Testes"* e lá será gerada uma pasta contendo o projeto.

  ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/folder.png)

* Em sequência precisamos definir um compilador, que no nosso caso será o ***"GNU GCC Compiler"*** e em seguida, clicamos no botão *"Finish"*.

  ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/compiler.png)

* Agora precisamos criar um novo arquivo, mas um arquivo especifico que a IDE entenda que é um arquivo que servirá de base para nosso programa...

  * Clicando em *"File"*
  * e depois em *"New"*
  * e por fim clicamos em *"From template..."*

  ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/file.png)

* Em sequência precisamos definir como este arquivo será, então clicamos em *"Files"*, depois vamos marcar a opção *"C/C++ source"* e damos continuidade clicando em *"Go"*

* Depois em Next...

  ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/next.png)

* Agora na tela seguinte, marcamos o tipo de Linguagem que vamos usar, que neste caso, marcamos *"C++"* e prosseguimos clicando em *"Next"*

* E por fim, damos um nome ao arquivo *não precisa de uma extensão específica* e clicamos no botão com *"três pontinhos (...)"*  e depois clicar no botão *"Save"*, e após isso, marcamos uma opção entre *"Debug"* ou *"Release"* ou quem sabe as duas, mas precisa ter ao menos uma, senão não será possível compilar o programa depois, feitos estes passos já será possível finalizar a criação do nosso arquivo e por fim criarmos nosso primeiro programa em C++.novamente em *"Next"*.

  ![](https://github.com/bynmboy/gcc-windows-guide/tree/main/img/setname.png)

* E por fim testificamos o sucesso na preparação do ambiente criando nosso primeiro programa em C++ e mandamos rodar clicando no botão com um triângulo *"que na verdade é uma seta"*  verde sobreposta à uma engrenagem amarela e será executado no *"prompt"* do windows a mensagem *"Hello World!"* :) 



#### Parabéns, agora já pode começar seus estudos sobre a linguagem C++

