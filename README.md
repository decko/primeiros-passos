# Primeiros Passos
Tudo o que você queria saber sobre boas práticas de desenvolvimento em um órgão público mas tinha medo de perguntar.

## O que é isto?
Este documento é uma tentativa de fornecer as bases para o iniciar o desenvolvimento dos sistemas do Ministério da Cultura. A idéia é que com o menor esforço possivel, você consiga adequar seu código a um conjunto de boas práticas e verificações automatizadas que te auxilie no dia a dia do desenvolvimento.

## Por onde começar
Primeiramente..., leia o README.md do projeto com o qual você vai trabalhar. Ele deve conter requisitos minimos para desenvolvimento e execução, com instruções necessárias para construir, instanciar e manter um ambiente de desenvolvimento com o que for necessário. Deve conter também os requisitos e informações sobre como rodar o software em um ambiente de produção.

## O que devo usar?
Os desenvolvedores tem liberdade e autonomia para utilizarem as ferramentas com as quais se sintam confortavéis, desde que respeitem o conjunto de regras decididas em consenso sobre a base de código. Assim, você é livre para utilizar o editor/IDE que quiser, desde que respeite coisas como formatação/identação de código, verificações de "linters", dentre outros acordos comuns.

### Editores/IDEs

Nome|Descrição
----|-----------
vim/neovim| VIM é um editor clássico do universo do UNIX e possui um modo de operação muito peculiar. Pode apresentar uma curva de aprendizagem acentuada para quem está começando na área, fato que é compensado pela possibilidade de personalização e desempenho em ambientes com poucos recursos. Prática comum da comunidade é compartilhar os arquivos de configuração, como pode ser visto [aqui.](https://gitlab.com/decko/dotfiles/raw/master/.config/nvim/init.vim)
Visual Studio Code| O vscode é um projeto de código aberto da Microsoft que fornece um ambiente de programação bem personalizavél com muitos plugins e temas. Roda em Windows, OSX e Linux.

### Formatação Geral de Código

Nome|Descrição
-----|----------
editorconfig| O editorconfig é um formato de arquivo e uma coleção de plugins para diversos editores que permite a centralização de regras simples de identação de códigos. Cada projeto pode ter uma configuração especifica sobre quantos espaços ou se uma tabulação deve ser o caractere que define os blocos de código. Um exemplo pode ser encontrado neste repositório.
