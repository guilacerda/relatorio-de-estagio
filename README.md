# Template Relatório de Estágio Obrigatório FGA-UnB
 
Template para Relatório de estágio obrigatório adaptado do template de Trabalhos de Conclusão de Cursos (TCC) na Faculdade do Gama (FGA) em Latex. O template de TCC foi
desenvolvido e adaptado pelo professor Edson Alves <edsomjr@gmail.com> e licenciado em Creative Commons Atribuição 3.0: http://creativecommons.org/licenses/by/3.0/ .
O template para Relatório de estágio obrigatório  FGA-UnB foi adaptado por João Paulo Nunes Soares.

## Utilizando o template no Overleaf

Caso deseje editar este documento no Overleaf, siga os seguintes passos:

1. Realize o download do repositório no formato **.zip**.

2. No Overleaf, na página "Seus Projetos" clique em *Novo Projeto*(localizado no canto superior esquerdo) e selecione a opção *Carregar Projeto*.

3. Selecione a pasta que você realizou o download no passo 1.

4. Após o projeto carregar, clique em **Menu**(localizado no canto superior esquerdo.

5. Na seção Configurações, selecione o arquivo **main.tex** como Documento Principal.

6. Compile o projeto.


## Instalando o abnTeX2 para compilar na máquina

### Ubuntu 12.10 ou superior

Uma vez que a versão recomendada do Tex Live é a 2012 ou superior, o processo de
instalação via apt-get funciona apenas a partir da versão 7.0 do Debian (também 
conhecida como Wheezy) e suas derivadas, como por exemplo Ubuntu 12.10 (também 
conhecida como Quantal Quetzal), Linux Mint 14, entre outras.

Para instalar o abnTeX2 (e as respectivas dependências, como o próprio TeXLive) 
em uma distribuição Debian ou derivada, utilize a instalação via apt-get (ou 
outro gerenciador de pacotes que preferir):

Adicione a seguinte linha ao arquivo /etc/apt/sources.list:
	
	deb http://distrib.abntex2.googlecode.com/hg/debian/ testing main

Opcionalmente, adicione a linha abaixo caso deseje baixar os fontes:

	deb-src http://distrib.abntex2.googlecode.com/hg/debian/ testing main

Adicione a chave pública ao chaveiro do apt:

	$ wget -O - http://distrib.abntex2.googlecode.com/hg/debian/89C55467.asc|sudo apt-key add - 

Instale o abntex2:

	$ sudo apt-get update && sudo apt-get install abntex2

Para atualizar uma instalação já existente, feita a partir do repositório:
	
	$ sudo apt-get update && sudo apt-get upgrade

Após o processo de instalação, você poderá ler os manuais e testar os exemplos 
que estarão disponíveis nos diretórios /usr/share/doc/abntex2/pdf e 
/usr/share/doc/abntex2/latex respectivamente.

Fonte: https://code.google.com/p/abntex2/wiki/InstalacaoLinux

### Ubuntu 12.04 ou inferior

Conforme consta na página de [instalação do abnTeX2 em distribuições GNU/Linux](https://code.google.com/p/abntex2/wiki/InstalacaoLinux#Instala%C3%A7%C3%A3o_autom%C3%A1tica_do_TeX_Live_e_do_abnTeX2_(recomendado)
, a instalação via apt-get funciona apenas a partir da versão 12.10 do Ubuntu, 
pois é nela que está disponível a versão 2012 do Tex Live, que é a recomendada 
para utilização com o abnTeX2.

Para instalar o abnTeX2 no Ubuntu 12.04 é necessário, pelo menos, atualizar o 
Tex Live. Uma das formas possíveis é utilizando os pacotes existentes no 
repositório [texlive-backports](https://launchpad.net/~texlive-backports/+archive/ppa)
, conforme orientações abaixo.

Adicione o repositório texlive-backports, digitando o seguinte em um terminal:

	$ sudo add-apt-repository ppa:texlive-backports/ppa

Caso o pacote texlive do Ubuntu 12.04 já esteja instalado digite:
	
	$ sudo apt-get update && sudo apt-get upgrade

Caso o pacote texlive do Ubuntu 12.04 ainda não esteja instalado digite:

	$ sudo apt-get update && sudo apt-get install texlive

Outra forma de atualizar o Tex Live é manualmente, conforme descrito na página 
de [instalação do abnTeX2 em distribuições GNU/Linux](https://code.google.com/p/abntex2/wiki/InstalacaoLinux#Instala%C3%A7%C3%A3o_manual_a_partir_do_instalador_do_TUG)

Fonte: https://code.google.com/p/abntex2/wiki/FAQ#Por_que_eu_não_consigo_instalar_o_abnTeX2_no_Ubuntu_12.04_via_a

### Outras distribuições linux

Informações para instalar o abnTeX2 em outras distribuições linux:

https://code.google.com/p/abntex2/wiki/InstalacaoLinux

### Windows

Informações para instalar o abnTeX2 no Windows:

https://code.google.com/p/abntex2/wiki/InstalacaoWindows

### Mac OS

Informações para instalar o abnTeX2 no Mac OS X:

https://code.google.com/p/abntex2/wiki/InstalacaoMac

## Compilando

Para compilar o texto através do Makefile digite:

	$ make clean
	$ make


