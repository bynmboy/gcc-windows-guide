# Configuração básica para usar o Editor Nodepad++ para estudar C++

## Este guia irá de forma objetiva, mostrar como configurar o editor Notepad++ de forma
## que você consiga criar seus códigos, compilar, e executar através do terminal do
## Windows seus programas compilados.

* Primeiro, acesse o site do Notepad++ [aqui](https://notepad-plus-plus.org/).

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img1.png)

* Clique em "Downloads" e procure sempre entrar na opção mais atualizada, como mostrado em amarelo.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img2.png)

* A imagem seguinte, mostra opções para que você possa escolher e baixar e usar, 
  nos Sistemas 64bits, 32bits ou ARM 64bits

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img3.png)

* Baixado o instalador, basta abrir clicando duas vezes no arquivo de instalação baixado.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img4.png)

* Selecione o idioma de sua escolha e clique em "OK".

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img5.png)

* Na tela de "boas vindas" clique em "Próximo >".

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img6.png)

* Clique em "Eu Concordo" como mostrado em amarelo.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img7.png)

* Se preferir um diretório diferente do padrão, pode clicar no botão "Procurar..." 
  marcado de amarelo, escolher o diretório de sua escolha e depois em "Próximo >".
  
![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img8.png)

* Caso queira selecionar um tipo específico de instalação, fique a vontade e depois
  clique em "Próximo >".
  
 ![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img9.png)
 
 * Aqui eu marquei a opção de criar um ícone na área de trabalho, e depois cliquei em "Instalar".
 
 ![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img10.png)
 
 * Pode desmarcar a opção de "Executar o Notepad++" se assim preferir, e depois clicar em "Concluir".

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img11.png)

* Aqui ele irá abrir sozinho se deixou marcado a opção para tal, e você verá ele como na imagem abaixo.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img12.png)

* Para que possamos compilar e executar nossos programas, é importante que já tenha um compilador
  instalado, pode usar o [LLVM](https://github.com/bynmboy/linguagemcpp/blob/main/windows-setup-llvm.md)
  mas o LLVM precisa do Visual Studio Code instalado com o compilador que ele usa, ou pode usar o g++
  do pacote GCC que explico [aqui](https://github.com/bynmboy/linguagemcpp/blob/main/windows-setup-gcc-codeblocks.md).
  Clique em "Plugins" e depois "Gerenciador de plugins..." como a imagem mostra em amarelo.
  
![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img13.png)

* Na janela que se abre, pesquise por "NppExec" clique em "Próximo", marque a opção correspondente
  e depois clique em "Instalar".
  
![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img14.png)

* O editor irá avisar que será necessário reiniciar o editor.

![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img15.png)

* Com o editor já reiniciado e com o plugin já instalado, crie uma pasta com nome "teste-cpp"
  na área de trabalho apenas para teste, dentro crie um arquivo com nome "program.cpp" que será
  responsável por ser o arquivo que se tornará o nosso programa de teste, pode criar manualmente
  ou através do editor nas opções do menu "Arquivo" aproveite e gaste um tempo olhando as opções
  e conhecendo o editor. Com o arquivo aberto no editor, apenas copie o código que verá na imagem.
  
  ```cpp
    $include <iostream>
    
    int main()
    {
      std::cout << "Funcionou!" << std::endl;
      system("PAUSE");
      return 0;
    }
  ```
  
![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img16.png)

* Vá para o menu "Plugins" depois em "NppExec" e marque a opção "Follow $(CURRENT_DIRECTORY)"
  para que os comandos do NppExec sejam feitos no diretório raiz do projeto.
  
![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img17.png)

* Em seguida, precione a tecla "F6" do seu teclado, e uma nova janela será aberta, adicione
  o código que veja a seguir para que o editor possa chamar o compilador, usar o arquivo
  atual como argumento, e em seguida passar o nome do arquivo sem a extensão do mesmo
  para que seja compilado, e criado o binário do código anterior, e em seguida executar o
  binário.
  
  ```
    C:\TDM-GCC-64\bin\g++.exe "$(FULL_CURRENT_PATH)" -o $(NAME_PART)
    NPP_RUN $(CURRENT_DIRECTORY)\"$(NAME_PART).exe"
  ```
  Clique em "Save..." na pequena janelinha, dê um nome para ele como eu fiz, depois clique
  em "Save" e por fim em "OK".
  
![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img18.png)

* Neste momento o editor irá seguir os passo que citei antes, e será possível ver o terminal
  do Windows mostrando a mensagem que mandamos o programa mostrar para nós.
  
![Alt_text](https://github.com/bynmboy/linguagemcpp/blob/main/npp-C%2B%2B/img19.png)


## Muito bem, agora você pode usar o Notepad++ para estudar a Linguagem C++ sem consumir
## muitos recursos do seu sistema, no exemplo que fiz, usei o gcc mas você pode instalar
## o Visual Studio Code, depois o LLVM e compilar tranquilamente, ou pode usar o GCC como
## fiz neste guia, boa sorte e bons estudos!

Att. Fabio Carneiro
