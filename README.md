# Sistema de Gestão do Mercadão

Projeto desenvolvido no âmbito da unidade curricular de Concepção e Desenvolvimento de Sistemas de Informação.

## Contexto

O trabalho foi desenvolvido em várias fases. Na primeira fase, a nossa equipa realizou a análise do sistema e produziu os diagramas de processos e de classes. 
Na fase seguinte, desenvolvemos o protótipo e o design da interface no Figma.

Durante a fase de desenvolvimento, os projetos foram redistribuídos entre os grupos. 
Por esse motivo, a implementação OutSystems incluída neste repositório corresponde ao sistema especificado originalmente por outro grupo.
A análise e o design incluídos neste repositório correspondem ao trabalho realizado pela nossa equipa nas fases anteriores, com base no
enunciado do projeto.

A implementação foi desenvolvida pela nossa equipa com base nos diagramas, requisitos e protótipos fornecidos pelo outro grupo.
Esta distinção é apresentada para identificar corretamente a autoria dos diferentes elementos do projeto.

## Organização do sistema

O sistema está dividido em duas áreas principais:

- **Frontoffice** — área destinada aos candidatos e restantes utilizadores externos;
- **Backoffice** — área destinada aos colaboradores envolvidos no processo de recrutamento.

As duas áreas possuem páginas de entrada, funcionalidades e fluxos de navegação diferentes, de acordo com o perfil do utilizador.

### Frontoffice

No Frontoffice, o candidato pode:

- criar e consultar o seu perfil;
- consultar as vagas publicadas;
- consultar os detalhes de uma vaga;
- submeter candidaturas;
- anexar documentação;
- acompanhar o estado das candidaturas submetidas.

### Backoffice

O Backoffice permite aos colaboradores gerir propostas de trabalho e acompanhar o processo de recrutamento.

## Conteúdo do repositório

- `docs/fase-1-analise/` — diagramas de processos, diagramas de classes e documentação de análise realizados pela nossa equipa;
- `docs/fase-2-design/` — protótipos, screenshots e decisões de design desenvolvidos pela nossa equipa;
- `outsystems/` — exportações dos módulos OutSystems desenvolvidos pela nossa equipa durante a fase de implementação;

A documentação das fases de análise e design representa a idealização inicial da nossa equipa. 
A implementação OutSystems foi realizada com base na especificação e no design fornecidos pelo outro grupo após a redistribuição dos projetos.

## Perfis e permissões

O sistema utiliza diferentes perfis de utilizador, com permissões específicas no Backoffice.

### Candidato

O candidato utiliza principalmente o Frontoffice e pode:

- criar e consultar o seu perfil;
- consultar vagas publicadas;
- consultar os detalhes das vagas;
- submeter candidaturas;
- acompanhar o estado das suas candidaturas.

### Gestor de Loja

O Gestor de Loja pode:

- criar propostas de trabalho;
- submeter propostas para revisão;
- consultar propostas e vagas;
- acompanhar os candidatos associados às vagas;
- encerrar vagas.

### Direção de RH

A Direção de RH pode:

- consultar propostas submetidas;
- aprovar ou rejeitar propostas;
- pedir alterações às propostas;
- consultar vagas e candidatos;
- aceder à área de dados do sistema;
- editar determinados dados de suporte.

### Técnico de RH

O Técnico de RH pode:

- consultar propostas e vagas;
- pedir alterações às propostas;
- publicar propostas aprovadas;
- validar informação dos candidatos;
- acompanhar o processo de avaliação;
- registar avaliações e entrevistas;
- acompanhar o progresso das candidaturas.

As permissões são controladas de acordo com o perfil do utilizador. 
Assim, determinadas páginas e ações apenas ficam disponíveis para os utilizadores com autorização para as executar.
Por exemplo, a área de dados está limitada à Direção de RH, enquanto as ações de publicação e avaliação dependem do perfil do utilizador e do estado da proposta ou candidatura.

## Fluxos principais

### Fluxo de uma proposta de trabalho

1. O Gestor de Loja cria uma proposta.
2. A proposta é submetida para revisão.
3. A Direção de RH aprova, rejeita ou pede alterações.
4. O Técnico de RH valida e publica a proposta.
5. A vaga fica disponível no Frontoffice.
6. O Gestor de Loja pode encerrar a vaga.

### Fluxo de uma candidatura

1. O candidato cria ou utiliza o seu perfil.
2. Consulta as vagas disponíveis.
3. Submete uma candidatura.
4. A candidatura é validada e avaliada no Backoffice.
5. São registadas as avaliações e entrevistas necessárias.
6. A candidatura avança pelos estados correspondentes até à decisão final.

## Tecnologias e ferramentas

- OutSystems
- Figma
- UML
- BPMN

## Execução do projeto

Os ficheiros `.oml` correspondem aos módulos exportados do OutSystems e podem ser utilizados para importar o projeto para um ambiente OutSystems compatível.

A execução poderá depender da configuração do ambiente, das entidades, dependências e serviços externos utilizados pelo projeto.
O ambiente online utilizado durante o desenvolvimento já não está disponível devido às limitações dos Personal Environments da OutSystems.

Não são incluídas neste repositório credenciais de acesso a nenhum ambiente online.
Para compreender a solução, estão disponíveis os ficheiros `.oml`, a documentação, os diagramas e os screenshots.

## Nota de autoria

Os ficheiros estão organizados de acordo com as diferentes fases do trabalho.

A análise da fase 1 e o design da fase 2 foram realizados pela nossa equipa, com base na idealização do sistema definida a partir do enunciado.

Durante a fase de desenvolvimento, os projetos foram redistribuídos.
A implementação OutSystems deste repositório foi desenvolvida pela nossa equipa com base nos diagramas, requisitos e protótipos fornecidos pelo outro grupo.
