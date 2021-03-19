Tutorial Básico Git
=======================

**Git** é um sistema de controle de versões, usado principalmente no desenvolvimento de software, mas pode ser usado para registrar o histórico de edições de qualquer tipo de arquivo.

Já o [GitHub](https://github.com/) é uma plataforma de hospedagem de código-fonte e arquivos com controle de versão usando o Git.


## Passo Inicial: Instalação do Git
* Baixar e instalar o [Git for Windows](https://git-scm.com/download/win)
* Seguir as configurações recomendadas durante a instalação

## Monitorar uma pasta com o Git
* Ao clicar com o botão direito do mouse em qualquer pasta, clique em **Git Bash Here**
* Comando para iniciar o repositório: `git init`
* Configurar as credenciais do autor: `git config user.email "seuemail@exemplo.com"` e `git config user.name "Seu Nome"`
* Depois é necessário adicionar os arquivos que serão monitorados: `git add --all`
* Ao realizar grandes modificações é recomendado criar um ponto para registro, chamado de **commit**: `git commit -m "comentários das alterações"`
* Observação: sempre antes de um commit é necessário adicionar os arquivos com o comando add

## Enviar a pasta do projeto para o GitHub
* Levando em conta que já seguiu os passos anteriores e agora você queira mandar esses arquivos para a "nuvem" do GitHub, basta seguir os passos:
* Caso o repositório ainda não exista no GitHub é necessário cria-lo através do [site](https://github.com/)
* Criar um ramo para seu projeto: `git branch -M main`
* Indicar o caminho do repositório no GitHub, exemplo: `git remote add origin https://github.com/senai914/Tutorial-Git.git`
* E para enviar de fato ao GitHub: `git push -u origin main`
* Caso o repositório já exista e queira apenas enviar a alteração: adicione os arquivos, gere o commit e dê o comando push

## Baixar as alterações do projeto no GitHub para o PC
* O comando `git pull` atualiza a sua pasta local com a última versão que está no GitHub
