# Preparando o ambiente para Programar em C++ no Windows 

## Instalação LLVM um frontend para compilar códigos C, C++, Fortran entre outros.

* Acesse a página de Downloads do projeto LLVM [aqui](https://releases.llvm.org/download.html)
* Acesse a home do projeto para saber mais sobre [aqui](https://llvm.org/)
* Se preferir consultar a documentação do projeto [aqui](https://llvm.org/docs/GettingStarted.html#checkout)
* A versão que uso neste momento é a 14.0.0, para baixar para Window ou outra opção de S.O. [aqui](https://github.com/llvm/llvm-project/releases/tag/llvmorg-14.0.0)
* Se preferir para Windows 64Bits [aqui](https://github.com/llvm/llvm-project/releases/download/llvmorg-14.0.0/LLVM-14.0.0-win64.exe)
* Se preferir para Windows 32Bits [aqui](https://github.com/llvm/llvm-project/releases/download/llvmorg-14.0.0/LLVM-14.0.0-win32.exe)

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img1.png)

* Uma vez que o download foi concluído com sucesso, precisamos apenas dar um click duplo sobre o ícone do instalador e aceitar as permissôes de execução do programa.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img2.png)

* Em seguida será carregada uma janelinha mostrando o progresso do carregamento do instalador.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img3.png)

* Na tela de Boas Vindas, precisamos apenas clicar em "Próximo >".

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img4.png)

* Em seguida, concordar com os termos, ou não, você que decide, mas para continuar com a instalação precisa clicar em "Eu Concordo".

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img5.png)

* Aqui ocorre algo intrigante, mesmo selecionando a opção marcada com marca texto em amarelo, selecionando para que seja adicionada ao PATH para todos os usuários poderem ter acesso ao clang, ainda assim não foi feito, mas mostro ainda neste guia como fazê-lo manualmente aqui no Windows 11. Caso queira adicinar um ícone à área de trabalho, marque a opção que tem um "?" em vermelho, e prossiga com a instalação clicando em "Próximo >".

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img6.png)

* Caso queira alterar o caminho destino original de instalação. clique no botão "Procurar..." marcado em amarelo, e busque um lugar de sua escolha, mudando ou não, continue a instalação clicando em "Próximo >" como mostrado em amarelo na imagem.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img7.png)

* Clique em "Instalar" marcado de amarelo para de fato iniciarmos a instalação.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img8.png)

* Em seguida, apenas aguarde o progresso de instalação avançar até ser finalizado.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img9.png)

* Finalizado, apenas clique no botão "Concluir" marcado em amarelo.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img10.png)

* Para adicionarmos o compilador no PATH do Sistema para que o mesmo possa ser acessado pelo terminal, precisamos abrir o "Meu Computador" tarefa que qualquer usuário Windows sabe muito bem como fazer, visualizar o ícone "Este Computador" na lateral esquerda do gerenciador de arquivos do Windows, clicar com o botão direito do mouse, e com o menu suspenso de opções aberto, clicar com o botão esquerdo na opção "Propriedades" como marcado na imagem.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img11.png)

* Visualize a opção "Configurações avançadas do sistema" como mostrado em amarelo na imagem abaixo.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img12.png)

* Clique em "Variáveis de Ambiente...".

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img13.png)

* Dentro da "caixa" de opção de "Váriaveis do sistema" procure por "Path" como mostrado na imagem em amarelo, e em seguida, selecione ele clicando uma vez com o botão esquerdo do mouse, e em seguida clique em "Editar.." como mostrado.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img14.png)

* Na imagem abaixo, podemos conferir que não foi gerado a inclusão do LLVM no nosso Path do sistema.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img15.png)

* Para inserir um novo diretório no PATH do Windows, para que seus executáveis possam ser "vistos" pelo sistema, precisamo clicar no botão "Novo" marcado em amarelo, e poderemos incluir manualmente o caminho de qual diretório queremos acrescentar.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img16.png)

* Abra o nagevador de arquivos do Windos, e como mostrado na imagem abaixo, procure o caminho do diretório que o instalador do LLVM construiu, aqui no meu caso esse caminho é "C:\Program Files\LLVM" precisamos dos binários do compilador, que ficam na pasta denominada de "bin", como mostrado com uma marcação em amarelo.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img17.png)

* Abra a pasta "bin" clique no link de diretórios que será alterado pelo caminho absoluto, clique com o botão direito e copie este link, como mostrado em amarelo.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img18.png)

* De volta a janela de inclusão de novos diretórios ao Path do sistema, cole o caminho absoluto da pasta do LLVM/bin como mostrado anteriormente, em seguida clique em "OK".

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img19.png)

* A janela será fechada, voltando para a janela anterior, basta clicarmos em "OK" novamente.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img20.png)

* E na janela de "Propriedades do Sistema", novamente clicamos em "OK".

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img21.png)

* Para confirmação de que o nosso compilador, está de fato visível em nosso Sistema, abra o menu de aplicativos do Windows, e pesquise por "terminal" como mostrado na imagem, e abra-o.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img22.png)

* E por fim, digite "clang" que é o nosso compilador para códigos da linguagem C, e tecle "Enter", na imagem a seguir, será mostrado o erro: "clang: error: no input files" informando que não foi passado nenhum arquivo como argumento para o compilador clang, então podemos confirmar que o mesmo, já pode ser acessado pelo terminal, e usado em diversos editores de texto que nos permita compilar diretamente nele, onde precisamos informar qual compilador queremos.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/image-llvm-windows/img23.png)

## Muito bem, se tudo deu certo para você, agora você pode iniciar seus estudos da Linguagem de programação C e C++ no seu Windows!

Att. Fabio Carneiro
