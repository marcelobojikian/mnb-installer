<h1 align="center">
    MNB Installer - GUI v1.0
</h1>

<h4 align="center">
  Gerenciador de scripts de instalação por categorias
</h4>

<p align="center">
  <img alt="License" src="https://img.shields.io/static/v1?label=license&message=MIT">
</p>

<p align="center">

  <a href="https://github.com/marcelobojikian" target="_blank">
    <img alt="Feito por Marcelo Nogueira" src="https://img.shields.io/badge/Feito%20por-Marcelo_Nogueira-informational">
  </a>
  <a href="https://github.com/marcelobojikian" target="_blank" >
    <img alt="Github - Marcelo Nogueira" src="https://img.shields.io/badge/Github--%23F8952D?style=social&logo=github">
  </a>
  <a href="https://www.linkedin.com/in/marcelobojikian/" target="_blank" >
    <img alt="Linkedin - Marcelo Nogueira" src="https://img.shields.io/badge/Linkedin--%23F8952D?style=social&logo=linkedin">
  </a>

</p>

<p align="center">
  <a href="#-projeto">Projeto</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-pre-requisitos">Pré-requisitos</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#-como-usar">Como usar</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licença">Licença</a>
</p>

<br>

## 💻 Projeto

Esse projeto foi criado com a finalidade de facilitar a instalação de programas 
frequentemente utilizados, configurar as estruturas padrão que utilizo executando 
scripts personalizados.

Os passos de instalação será:

<ol>
  <li>Selecionar uma categoria.</li>
  <li>Marque os programas que deseja instalar.</li>
  <li>Confirme operações.</li>
  <li>Instalar.</li>
  <li>Finalizar programa.</li>
</ol>

Ps. __Futuramente não será permitida a reinstalação dos softwares já instalados.__

## 🔖 Pre-requisitos

O sistema depende de alguns pacotes para funcionar.

Instalar __dialog__ :

| **sudo apt-get install dialog**

Antes da utilização é necessario criar as __pastas__ de cada categoria, com o seu respectivo nome, na pasta __src/etc/mnb/installer/bash__.
Após a criação das categorias, os scripts __bash__ deverão estar em sua correspondente __pastas__. Por padrão todos os scripts devem finalizar com __*.installer__.

Exmeplo de categoria:

| **src/etc/mnb/installer/bash/minhacategoria**

Exmeplo de bash:

| **src/etc/mnb/installer/bash/minhacategoria/node.installer**

| **src/etc/mnb/installer/bash/minhacategoria/java.installer**

## 🤔 Como usar

Para gerar o pacote __.deb__ execute:

| **bash mnb pack**

Após a execução do comando de empacotamento, o arquivo __mnb-installer.deb__ será criado na pasta __dist__.

Utilize o comando __dpkg -i__ para isntalar:

| **sudo dpkg -i dist/mnb-installer.deb**

Após a instalação do __mnb-installer.deb__ o comando __mnb-installer__ estará habilitado para uso, execute o comando e siga as instruções.

<p align="center">

  <img alt="Tela inicial" src="https://github.com/marcelobojikian/mnb-installer/blob/main/assets/introduce.png?raw=true"  width="600px" />

  <img alt="Seleção de categoria" src="https://github.com/marcelobojikian/mnb-installer/blob/main/assets/category.png?raw=true"  width="600px" />

  <img alt="Seleção de programas" src="https://github.com/marcelobojikian/mnb-installer/blob/main/assets/programs.png?raw=true"  width="600px" />

  <img alt="Confirmação de instalação" src="https://github.com/marcelobojikian/mnb-installer/blob/main/assets/install.png?raw=true"  width="600px" />

  <img alt="Andamento da instalação" src="https://github.com/marcelobojikian/mnb-installer/blob/main/assets/progress.png?raw=true"  width="600px" />

  <img alt="Finalização do programa " src="https://github.com/marcelobojikian/mnb-installer/blob/main/assets/final.png?raw=true"  width="600px" />

</p>

## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE.md) para mais detalhes.


