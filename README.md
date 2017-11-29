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



## 1. Git
![Git](images/branching.png)

### 1.1 Git Workflow

Cada um dos sistema possuem suas peculiaridade de abordagem das issues até o tratamento do projeto como um todo, o que acaba variando os métodos de gerenciamento de branchs e fluxos de trabalho. Porém caso o sistema não possua o seu flow específico recomendamos o "[the simple guide](http://rogerdudler.github.io/git-guide/)" como default.

### 1.2 Commit messages

Ter um bom guide-line para a criação de commits deixa o trabalho com o git mais fácil, e prático para colaborações ([Fonte](https://chris.beams.io/posts/git-commit/#seven-rules)):

* Separe o assunto do corpo com uma nova linha entre as duas

  _Por quê?_
  > Git é inteligente o suficiente para distinguir a primeira linha do seu commit como um assunto. De fato, se você tentar git shortlog, ao invés de git log, você vai ver um longa lista de mensagem de commits, consistindo de id do commit e o assunto.

* Limite o assunto em 50 caracteres e o conteúdo do corpo em 72 caracteres.

  _Por quê?_
  > As mensagem de commit precisam ser breves e focadas, não é lugar para detalhes demais. [Leia mais...](https://medium.com/@preslavrachev/what-s-with-the-50-72-rule-8a906f61f09c)

* Capitalize a linha de assunto.

* Não escreva o assunto de modo temporal.
 >ex: "Fix - corrigindo bug da migração de ontem"

* Escreva sempre o assunto no [imperativo](https://pt.wikipedia.org/wiki/Modo_imperativo).

 _Por quê?_
 >Em vez de escrever mensagens que dizem o que um commit fez. É melhor considerar essas mensagens como as instruções para o que será feito após o commit ser aplicado no repositório.

* Use o corpo para explicar **o quê** e **porquê**, ao invés de **como**.



## 2. Documentação
![documentação](images/documentation.png)

* Para projetos com mais de um repositório, disponibilizem links neles nos respectivos `README.md` de cada um.

* Mantenha o `README.md` atualizado a medida que o projeto evolui.

* Caso possuam ferramentas de discussão (RocketChat, Telegram, Slack e etc..) de qualquer natureza sobre o sistema, disponibilizem no `README.md`.

* Não use comentários para se desculpar de um código ruim. Mantenha o código limpo (Não use `@TODO`, provavelmente você não irá refazer).

* Não use clean code como desculpa para não documentar.

* Em uso mínimo, mantenha apenas comentários relevantes no código.


#### [Referência base](https://github.com/wearehive/project-guidelines/).
