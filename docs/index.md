---
layout: default
---
# [1.](#header-1) Objetivo

Desenvolver um Sistema de protocolo de documentos, denominado Zelda, o qual é um protótipo do Sistema SAMUS. Com a finalidade de levantar os principais pontos relacionados ao desenvolvimento do projeto real, no que tange tecnologias e documentações relacionadas. Para que a experiência de desenvolvimento seja a mais branda possível, de forma a não ocorrer atrasos inesperados por ausência de conhecimento de determinada tecnologia, ou até mesmo, necessidade de conhecimento de funcionamento de processos.

# [2.](#header-1) Requisitos
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
 |RNF008		          |Telas separadas para funcionario e lotação| não tem |

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

## [3.](#header-2) Análise de Projeto

O projeto segue esquematizado de na forma de Entidade e Relacionamento, onde as principais entidades (setor,funcionário,usuário) são postas em tabelas no modelo físico do BD. Onde cada tabela tem seus atributos específicos em cada coluna deixando assim populado todas as informções do sistema referente as entidades envolvidas do sistema.

## [3.1.](#header-3) Tabela de Setor

A tabela  do setor, tem os seguintes atributos: setor_id, setor_nome, setor_situação, setor_pai.
Na coluna setor_id, ficam armazenados os dados referentes a identificação de cada setor, onde cada setor é identificado de forma única, ou seja, o setor_id é uma chave primária.

Na coluna setor_nome, ficam armazenados os dados referentes ao nome de cada setor, pois cada setor tem que ter um nome.

Na coluna setor_situação, ficam armazenados os dados referentes a situação de cada setor, ele é responsável por indicar o se o setor está ativo ou não.

Na coluna setor_pai, ficam armazenados os dados o id do setor_pai, ou seja ele recebe um valor inteiro, identificando o setor superior de cada setor que está abaixo da hieráquia.

|     setor_id     | setor_nome                                 | setor_pai | setor_situacao    |
|:---------------- |------------------------------------------- |---------- |-----------------  |
|     UEA00001     | Reitoria                                   |           |        1          |
|     UEA00002     | Gabinete do Reitor                         | UEA00001  |        1          |
|     UEA00003     | Gabinete do Vice-Reitor                    | UEA00001  |        1          |
|     UEA00004     | Pró-Reitoria de Planejamento               | UEA00001  |        1          |
|     UEA00005     | Pró-Reitoria de Administração              | UEA00001  |        1          |
|     UEA00006     | Pró-Reitoria de Ensino de Graduação        | UEA00001  |        1          |

## [3.2.](#header-3) Tabela de Usuário
A tabela usuário, tem os seguintes atributos : usuario_id, usuario_login, usuario_senha, usuario_logado e usuario_admin

Na coluna usuario_id, ficam armazenados os dados referentes a identificação de cada usuário,onde esse dado é uma chave primária e irá guardar uma identificação de cada usuário cadastrado no banco de dados.

Na coluna usuario_login, ficam armazenados os dados referentes ao login que o usuário cadastrou

Na coluna usuario_senha, ficam armazenados a senha que o usuário cadastrou

Na coluna usuario_logado, irá definir se o usuário está logado, definindo como 1 caso esteja logado ou 0 caso contrário

Na coluna usuario_admin, irá guardar se o usuário é administrador ou não.

|     usuario_id     | usuario_login           | usuario_senha  | usuario_admin |
|:---------------- |-------------------------- |----------------|---------------|
|         2              | Andréa              | andrea@123     |     1         |                   
|         3              | Antônio             | antonio@123    |     1         |
|         4              | Cássio              | cassio@123     |     1         |
|         5              | Charles             | charles@123    |     1         |
|         6              | Clairon             | clairon@123    |     1         |
|         7              | Cláudio             | claudio@123    |     1         |


## [3.3.](#header-3) Tabela de Funcionário
A tabela funcionário, tem os seguintes atributos : funcionario_id,funcionario_nome, funcionario_situacao

Na coluna funcionario_id, ficam armazenados os dados referentes a identificação de cada funcionário sendo esse valor criado como uma chave primária, que determina um valor único no banco de dados.

Na coluna funcionário_nome, ficam armazenados os nomes de cada usuário cadastrado no sistema

Na coluna funcionario_situacao, ficam armazenados a situaçãso de cada funcionário sendo o valor 1 o valor inicial que determina funcionário ativo e caso haja uma alteração na situação do funcionário ele recebe o valor 0 para inativo.

|     funcionario_id     | funcionario_nome                | funcionario_situacao |
|:---------------------- |-------------------------------- |--------------------- |
|         2              | Andréa Fragata                  |         1            |
|         3              | Antônio Estanislau              |         1            |
|         4              | Cássio Bernardes                |         1            |
|         5              | Charles Luiz                    |         1            |
|         6              | Clairon Lima                    |         1            |
|         7              | Cláudio Gonçalves               |         1            |

* * *

## [4. ](#header-2)Implementação

Na sua versão atual, o sistema contém 6(seis) telas, que compõem o módulo Zelda. Onde estas são:

- [Login](https://docs.google.com/a/uea.edu.br/document/d/1L7sYBf0ZaKGEKfPf_h7y5uq32a7BxG4NOdgCQpNOZrY/edit?usp=sharing)
- [Administrador](https://drive.google.com/a/uea.edu.br/file/d/0B09Ckx-J88eyUE5feHprT1htUm8/view?usp=sharing)
- [Usuário](https://drive.google.com/a/uea.edu.br/file/d/0B09Ckx-J88eyQ2pfVXFoMWhra2M/view?usp=sharing)
- [Cadastro de funcionários](https://drive.google.com/a/uea.edu.br/file/d/0B09Ckx-J88eybXJaMU1zR1NiREk/view?usp=sharing)
- [Cadastro de setor](https://drive.google.com/a/uea.edu.br/file/d/0B09Ckx-J88eyQUd2djdIaE1ZVU0/view?usp=sharing)
- [Cadastro de usuário](https://drive.google.com/a/uea.edu.br/file/d/0B09Ckx-J88eyMGVoTkd6UGdZZms/view?usp=sharing)
- [Listagem de funcionários](https://drive.google.com/a/uea.edu.br/file/d/0B09Ckx-J88eya2J0enU5d09iaUk/view?usp=sharing)
- [Listagem de setores](https://drive.google.com/a/uea.edu.br/file/d/0B09Ckx-J88eya2J0enU5d09iaUk/view?usp=sharing)
- [Listagem de usuários](https://drive.google.com/a/uea.edu.br/file/d/0B09Ckx-J88eydTRDV0V2WkhZaHM/view?usp=sharing)

Segue abaixo a iteração entre as telas do sistema.

![](images/Diagrama.png?raw=true)

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
