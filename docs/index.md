---
layout: default
---
# [1.](#header-1) Objetivo

Desenvolver um Sistema de protocolo de documentos, denominado Zelda, o qual é um protótipo do Sistema SAMUS. Com a finalidade de levantar os principais pontos relacionados ao desenvolvimento do projeto real, no que tange tecnologias e documentações relacionadas. Para que a experiência de desenvolvimento seja a mais branda possível, de forma a não ocorrer atrasos inesperados por ausência de conhecimento de determinada tecnologia, ou até mesmo, necessidade de conhecimento de funcionamento de processos.

# [2.](#header-1) Requisitos
Os requisitos funcionais tratam de funções que o sistema deve fornecer, como o sistema deve se comportar a entradas e a determinadas situações (PRESSMAN, 2001).

Em outras palavras, descrevem a funcionalidade ou serviço que se espera que o sistema forneça. Dependendo do tipo de software do requisito a ser descrito é possíveis criar subgrupos de requisitos funcionais, normalmente subdivididos como requisitos funcinais de usuário e do sistema (SOMERVILLE, 2001).

## [2.1.](#header-2) Não Funcionais
 Requisitos não funcionais são os requisitos sob os quais o sistemas devem operar, podendo conter restrições sobre o software em si ou mesmo sobre o seu processo de desenvolvimento

 |     Codigo         | Nome                    | Descrição     |
 |:-------------------|:------------------------|:--------------|
 |RNF001              |Uso do Flask/Bootstrap   |Para o desenvolvimento deste projeto deve ser utilizado entre outras feramentas Flask e Bootstrap      |
 |RNF002              |Uso do GitHub            |Todo o codigo fonte deve ser versionado por meio do GitHub |
 |RNF003              |Codigo fonte padronizado |Todo o codigo fonte deve seguir o padrão previamente estabeecido    |
 |RNF004              |Uso do Trello            |Todas as tarefas do projeto devem ser organizadas por meio do Trello		|
 |RNF005              |Segurança		            |O sistema deve garantir que seus dados não sejam acessados por pessoas sem as devidas permissões      |
 |RNF006		          |URLs amigáveis	          |O sistema deve possuir URLs de de fácil leitura e intuitivas	|
 |RNF007		          |Usuario Adiministrador   |Apenas o usuario administrador pode acessar os funcionarios e os seus setores |
 |RNF008		          |Telas separadas para funcionario e lotação| ... |

* * *
## [2.2](#header-3) Funcionais
Os requisitos funcionais tratam de funções que o sistema deve fornecer, como o sistema deve se comportar a estradas e a determinadas situações (PRESSMAN, 2001).

## [2.2.1.](#header-4) Usuário
São os requisitos funcionais com os quais o usuário interage diretamente, de tal forma que sua participação ativa é necessária para que alguma ação seja efetuada pelo sistema.

|     Codigo         | Nome                    | Descrição     |
|:-------------------|:------------------------|:--------------|
| RF001              | Login unico             |O sistema deve permitir ao usuario que  entre no sistema por meio do seu login unico e senha       |
|RF002               | Cadastrar funcionarios  |O sistema deve permitir ao usuario cadastrar novos funcionarios   |
|RF003               | Cadastrar setor	       |O sistema deve permitir ao usuario cadastrar novos setores  |
|RF004               | Relacionar funcionario a setor                   |O sistema deve permitir ao usuario relacionar um funcionario a um setor    |
|RF005               | Cadastro de usuarios    |O sistema deve permitir ao usuario que se cadastre no sistema por meio de um login e senha |

* * *

## [2.2.2.](#header-4) Sistema
São os requisitos funcionais com os quais o usuário não interage diretamente, de modo que sua participação ativa não é necessária para que o sistema efetue alguma ação.

|     Codigo         | Nome                    | Descrição     |
|:-------------------|:------------------------|:--------------|
|RF006		     | Tela Admin	       |O sistema deve direcionar o adiministrdor para a tela de Administrador  |

* * *

## [](#header-2)Regras de Negócio

> Devido ao alto detalhamento das informações das regras de negócio, esta encontra-se nesta documentação somente em sua forma resumida. Para acessar o conteúdo completo, [clique aqui](https://docs.google.com/a/uea.edu.br/document/d/1L7sYBf0ZaKGEKfPf_h7y5uq32a7BxG4NOdgCQpNOZrY/edit?usp=sharing).

- Usuário
  - O usuário poderá fazer login;
    - Enquanto o usuário estiver logado, poderá fazer logout;
  - O usuário poderá visualizar seus dados;
- Administrador
  - O administrador poderá fazer login;
    - Enquanto o administrador estiver logado, poderá fazer logout.
  - O administrador poderá visualizar seus dados;
  - O administrador poderá listar usuários;
    - Nesta lista, o administrador poderá cadastrar, editar e desativar um ou mais usuários.
  - O administrador poderá listar funcionários;
    - Nesta lista, o administrador poderá cadastrar, editar e desativar um ou mais funcionários.
  - O administrador poderá listar setores;
    - Nesta lista, o administrador poderá cadastrar, editar e desativar um ou mais setores.


* * *

## [](#header-2)Diagrama de Casos de Uso

> Inserir aqui breve descrição, conforme fornecido pela equipe responsável.
Essa tabela pode ter mais de 3 colunas e mais de 6 linhas. Vai depender do que a equipe fornecer.

* Nome do Diagrama

![](endereçamento pro arquivo)

* Nome do Diagrama

![](endereçamento pro arquivo)

* Nome do Diagrama

![](endereçamento pro arquivo)

* Nome do Diagrama

![](endereçamento pro arquivo)

* Nome do Diagrama

![](endereçamento pro arquivo)

* Nome do Diagrama

![](endereçamento pro arquivo)

* * *

## [](#header-2)Análise de Projeto

> Inserir aqui breve descrição, conforme fornecido pela equipe responsável.
Essa tabela pode ter mais de 3 colunas e mais de 6 linhas. Vai depender do que a equipe fornecer.

Se for uma tabela pequena, utilizar:

|     Integrante     | Atividade               | Concluída |
|:-------------------|:------------------------|:----------|
| Thatielen Oliveira | Organização das tarefas |    SIM    |
| Thatielen Oliveira | Elaboração de planilhas |    SIM    |
| Thatielen Oliveira | Checagem das tarefas    |    NÃO    |
| Thatielen Oliveira | Checagem das tarefas    |    NÃO    |

Se for uma tabela muito grande, redirecionar para uma página contendo a tabela, utilizando:
[Tabela](www.google.com)

* * *

## [](#header-2)Implementação

> Recolhimento e apresentação das telas do sistema.

* Nome da Tela

![](endereçamento pro arquivo)

* Nome da Tela

![](endereçamento pro arquivo)

* Nome da Tela

![](endereçamento pro arquivo)

* Nome da Tela

![](endereçamento pro arquivo)

* * *

## [](#header-2)Planejamento e Gerência

#### [](#header-4)Equipe X

|     Integrante     | Atividade               | Concluída |
|:-------------------|:------------------------|:----------|
| Thatielen Oliveira | Organização das tarefas |    SIM    |
| Thatielen Oliveira | Elaboração de planilhas |    SIM    |
| Thatielen Oliveira | Checagem das tarefas    |    NÃO    |
| Thatielen Oliveira | Checagem das tarefas    |    NÃO    |

* * *

![](http://www.cdn.ueg.br/source/mobilidade_nacional_211/noticias/31283/uea.png)
