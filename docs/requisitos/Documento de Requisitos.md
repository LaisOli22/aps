Universidade de Pernambuco  
Escola Politécnica de Pernambuco  
Engenharia da Computação

**Documento de Requisitos**

**Grupo:**  
Bernardo Braga  
Giulia Buonafina  
Laís Oliveira  
Peri Macedo

**Recife**

**2025**

**Sumário**

**[1\. Introdução	](#introdução)**

[1.1. Escopo e Alinhamento Estratégico](#escopo-e-alinhamento-estratégico)

[1.2. Glossário	](#glossário)

[**2\. Visão Geral do Produto**](#2.-visão-geral-do-produto)

[2.1. Perspectivas do produto	](#2.1.-perspectivas-do-produto)

[2.2. Regras de negócio	](#2.2.-regras-de-negócio)

[2.3. Descrição dos atores do sistema	](#2.3.-descrição-dos-atores-do-sistema)

[**3\. Esquema de Usuários**](#3.-esquema-de-usuários)

[**4\. Objetivos de Negócio**](#4.-objetivos-de-negócio)

[**5\. Requisitos Funcionais (Casos de Uso)**](#5.-requisitos-funcionais-\(casos-de-uso\))

[\[RF001\] – Cadastrar](#[rf001]-–-cadastrar)

[\[RF002\] – Logar	](#[rf002]-–-logar)

[\[RF003\] – Recuperar senha	](#[rf003]-–-recuperar-senha)

[\[RF005\] – Candidatar-se à atividade	](#[rf005]-–-candidatar-se-à-atividade)

[\[RF006\] – Cancelar candidatura	](#[rf006]-–-cancelar-candidatura)

[\[RF007\] – Visualizar status do processo das atividades	](#[rf007]-–-visualizar-status-do-processo-das-atividades)

[\[RF008\] – Enviar documentos	](#[rf008]-–-enviar-documentos)

[\[RF009\] – Cancelar envio de documentos	](#[rf009]-–-cancelar-envio-de-documentos)

[\[RF010\] – Visualizar status dos documentos	](#[rf010]-–-visualizar-status-dos-documentos)

[\[RF011\] – Visualizar feedbacks	](#[rf011]-–-visualizar-feedbacks)

[\[RF012\] – Visualizar lista de alunos	](#[rf012]-–-visualizar-lista-de-alunos)

[\[RF013\] – Visualizar o aluno	](#[rf013]-–-visualizar-o-aluno)

[\[RF014\] – Visualizar lista de documentos	](#[rf014]-–-visualizar-lista-de-documentos)

[\[RF015\] – Visualizar documentos	](#[rf015]-–-visualizar-documentos)

[\[RF016\] – Validar documentos	](#[rf016]-–-validar-documentos)

[\[RF017\] – Adicionar feedback	](#[rf017]-–-adicionar-feedback)

[\[RF018\] – Remover feedback	](#[rf018]-–-remover-feedback)

[\[RF019\] – Visualizar histórico	](#[rf019]-–-visualizar-histórico)

[\[RF020\] – Registrar andamento da monitoria	](#[rf020]-–-registrar-andamento-da-monitoria)

[\[RF021\] – Remover andamento da monitoria	](#[rf021]-–-remover-andamento-da-monitoria)

[\[RF022\] – Enviar relatórios	](#[rf022]-–-enviar-relatórios)

[\[RF023\] – Cancelar envio de relatórios	](#[rf023]-–-cancelar-envio-de-relatórios)

[\[RF024\] – Cadastrar período de atividades	](#[rf024]-–-cadastrar-período-de-atividades)

[\[RF025\] – Editar período de atividades	](#[rf025]-–-editar-período-de-atividades)

[\[RF026\] – Editar perfil do usuário	](#[rf026]-–-editar-perfil-do-usuário)

[\[RF027\] – Reatribuir orientação	](#[rf027]-–-reatribuir-orientação)

[\[RF028\] – Buscar alunos por filtros	](#[rf028]-–-buscar-alunos-por-filtros)

[\[RF029\] – Arquivar atividades finalizadas	](#[rf029]-–-arquivar-atividades-finalizadas)

[\[RF030\] – Acompanhar prazos e pendências	](#[rf030]-–-acompanhar-prazos-e-pendências)

[\[RF031\] – Validar a elegibilidade do aluno	](#[rf031]-–-validar-a-elegibilidade-do-aluno)

[\[RF032\] \- Visualizar lista de relatórios	](#[rf032]---visualizar-lista-de-relatórios)

[\[RF033\] \- Visualizar relatórios	](#[rf033]---visualizar-relatórios)

[\[RF034\] – Obter metadados do documento	](#[rf034]-–-obter-metadados-do-documento)

[\[RF035\] – Obter metadados do relatório	](#[rf035]-–-obter-metadados-do-relatório)

[**6\. Requisitos não Funcionais** ](#6.-requisitos-não-funcionais)

[**7\. Diagrama de Casos de Uso**](#7.-diagrama-de-casos-de-uso)

[**8\. Referências**](#8.-referências)

1. # Introdução {#introdução}

Este projeto visa desenvolver um sistema para auxiliar alunos e professores no gerenciamento das atividades obrigatórias e complementares do curso, como TCC, Estágio e Monitoria. O sistema busca organizar documentos, etapas de aprovação e relatórios, facilitando o acompanhamento e cumprimento dos requisitos dessas atividades. Para os alunos será possível registrar e acompanhar o progresso das atividades acadêmicas (TCC, Estágio, Monitoria), enquanto professores e coordenadores possam realizar a validação e acompanhamento de documentos e relatórios.

1. ## Escopo e Alinhamento Estratégico {#escopo-e-alinhamento-estratégico}

   O Sistema de Gerenciamento de Atividades Acadêmicas (TCC, Estágio e Monitoria) é um projeto realizado para a disciplina de Análise e Desenvolvimento de Software.

   **O sistema permitirá:**

* Gerenciamento de usuários por perfil (Usuário não logado, Usuário logado, Aluno, Monitor, Estagiário, Aluno de TCC, Professor, Coordenador de curso e Funcionário administrativo);  
* Autenticação de usuários com controle de acesso baseado no tipo de usuário;  
* Cadastro e acompanhamento de projetos de TCC, Estágio e Monitoria;  
* Controle de etapas (Candidato, Executor, Relatório);  
* Envio de documentos digitais e relatórios conforme exigido por cada tipo de atividade;  
* Sistema de aprovação e feedback por parte dos professores e coordenadores;

  2. ## Glossário {#glossário}

* *TCC \- Trabalho de conclusão de curso*  
* *RF \- Requisito funcional*  
* *RNF \- Requisito não funcional*  
* *UC \- Caso de uso*  
* *RN \- Regras de negócio*  
* *Atividade \- (TCC, estágio e monitoria)*

# 2\. Visão Geral do Produto {#2.-visão-geral-do-produto}

## 2.1.	Perspectivas do produto  {#2.1.-perspectivas-do-produto}

O sistema será uma aplicação web independente, acessível por navegadores modernos, destinada a atender alunos de graduação, professores, coordenadores de curso e administradores acadêmicos. O sistema terá funcionalidades distintas por perfil de usuário, incluindo envio de documentos e relatórios, controle de prazos, aprovação e feedback.

## 2.2.	Regras de negócio {#2.2.-regras-de-negócio}

**Regras Gerais**

| ID | Regra de Negócio | Descrição |
| ----- | ----- | ----- |
| RN01 | Validação por perfil | Somente usuários autenticados por e-mail institucional e senha podem registrar ou validar atividades acadêmicas. |
| RN02 | Validação de aluno | Somente alunos matriculados podem registrar ou validar atividades acadêmicas. |
| RN03 | Acesso por perfil | Alunos apenas visualizam e editam suas próprias atividades; professores e coordenadores têm acesso apenas às atividades sob sua responsabilidade. |
| RN04 | Formato de documentos | Todos os documentos enviados devem estar em formato PDF e seguir os modelos da instituição. |
| RN05 | Notificações obrigatórias | O sistema deve notificar os envolvidos (alunos, professores, coordenadores) sobre prazos, alterações de status e solicitações pendentes. |
| RN06 | Controle de prazos | O sistema deve bloquear envios após a data-limite definida para cada etapa, salvo exceções autorizadas por administrador ou coordenador. |

**Estágio Curricular**

| ID | Regra de Negócio | Descrição |
| ----- | ----- | ----- |
| RN07 | Percentual mínimo para estágio obrigatório | O aluno só pode iniciar o estágio **obrigatório** após ter cumprido **pelo menos 60%** da carga horária total do curso. |
| RN08 | Percentual mínimo para estágio não obrigatório | O aluno pode iniciar o estágio **não obrigatório** após completar **pelo menos 10%** da carga horária total do curso. |
| RN09 | Documento inicial obrigatório | O aluno deve enviar obrigatoriamente o **Termo de Compromisso de Estágio** antes de iniciar a atividade. |
| RN10 | Relatórios periódicos | O aluno deve enviar um **relatório parcial a cada semestre** de estágio em andamento. |
| RN11 | Relatório final obrigatório | O aluno deve enviar um **relatório final de estágio** até 15 dias após o término da atividade. |
| RN12 | Validação de professor orientador | Todos os relatórios e documentos devem ser aprovados por um professor orientador antes de seguir para o coordenador. |
| RN13 | Rescisão de estágio | Caso o estágio seja encerrado antes do previsto, o aluno deve registrar uma **rescisão de contrato** e justificar no sistema. |

**Trabalho de Conclusão de Curso (TCC)**

| ID | Regra de Negócio | Descrição |
| ----- | ----- | ----- |
| RN14 | Requisito mínimo para TCC | O aluno só pode iniciar o TCC após completar **80%** da carga horária total do curso. |
| RN15 | Registro obrigatório de tema | O aluno deve registrar um **tema e orientador** para iniciar o TCC. |
| RN16 | Entregas obrigatórias | O aluno deve cumprir três entregas principais: **projeto (TCC1)**, **versão preliminar** e **versão final (TCC2)**. |
| RN17 | Avaliação final | A versão final do TCC deve ser avaliada por banca aprovada pelo coordenador do curso. |

**Monitoria**

| ID | Regra de Negócio | Descrição |
| ----- | ----- | ----- |
| RN18 | Disciplina cursada | O monitor já deve ter cursado a disciplina específica sob responsabilidade de um professor. |
| RN19 | Relatório obrigatório | O monitor deve enviar o **relatório semestral** conforme cronograma da disciplina. |
| RN20 | Frequência mínima | O aluno monitor deve ter **frequência mínima de 75%** nas atividades de monitoria para receber certificado. |
| RN21 | Validação pelo professor | O professor responsável deve aprovar o relatório e registrar a avaliação final do monitor. |

## 

## 2.3. Descrição dos atores do sistema {#2.3.-descrição-dos-atores-do-sistema}

| Tipo de ator | Descrição | Responsabilidades |
| ----- | ----- | ----- |
| Usuário não logado | Este ator representa um usuário que acessa funcionalidades básicas como cadastro, login e recuperação de senha. | Acessar a página de cadastro e login. Solicitar recuperação de senha. |
| Usuário logado | Ator genérico que representa qualquer usuário autenticado no sistema. |  |
| Aluno | Este ator representa um estudante regularmente matriculado, que pode estar envolvido em uma ou mais atividades (TCC, Estágio, Monitoria). | Candidatar-se em TCC, estágio e/ou monitoria, de acordo com regras de negócio. |
| Aluno de TCC | Este ator representa aluno envolvido na realização do Trabalho de Conclusão de Curso (TCC). | Enviar documentos (projeto, prévia, versão final). Acompanhar validações de professor e coordenador. |
| Estagiário | Este ator representa um aluno que está em estágio curricular supervisionado. | Enviar termos de compromisso, relatórios e documentos. Acompanhar validações de professor e coordenador. |
| Monitor | Este ator representa um aluno que auxilia um professor em atividades de ensino, com carga horária específica. | Registrar o andamento da monitoria. Submeter relatórios parciais e finais. Acompanhar o feedback do professor da disciplina. |
| Professor orientador | Ator que representa um docente responsável por acompanhar o desenvolvimento de uma ou mais atividades (TCC, Estágio ou Monitoria) dos alunos. | Validar registros e documentos submetidos por alunos. Fornecer feedbacks das atividades do seu aluno. Acompanhar progresso e status das atividades orientadas. |
| Coordenador de curso | Ator que representa um docente responsável por acompanhar e autorizar a finalização das atividades acadêmicas dos alunos. | Validar a elegibilidade de Alunos para/com as atividades. |
| Funcionário administrativo | Ator com funções operacionais e de apoio ao sistema, como gestão de prazos e organização documental. | Validar informações cadastrais dos usuários. Configurar regras e prazos institucionais. |

# 3\. Esquema de Usuários {#3.-esquema-de-usuários}

![][image1]  
                                                                                   

# 

# 4\. Objetivos de Negócio {#4.-objetivos-de-negócio}

| Objetivo de negócio | Descrição |
| :---- | :---- |
| Otimizar o acompanhamento das atividades acadêmicas | Permitir o gerenciamento centralizado de TCC, Estágio e Monitoria por meio de um sistema digital, otimizando os fluxos de submissão, aprovação e registro, reduzindo a burocracia e falhas de comunicação. |
| Oferecer rastreabilidade e transparência | Manter histórico completo das interações, documentos submetidos e decisões tomadas por professores e coordenadores, garantindo visibilidade para todos os envolvidos. |
| Facilitar a validação institucional das atividades | Padronizar os processos de envio e aprovação de documentos. |
| Promover a autonomia do aluno | Fornecer ao estudante uma plataforma com orientações, status e ferramentas que permitam acompanhar seu progresso sem depender de interações constantes com professores ou coordenação. |

# 

# 5\. Requisitos Funcionais (Casos de Uso) {#5.-requisitos-funcionais-(casos-de-uso)}

## \[RF001\] – Cadastrar {#[rf001]-–-cadastrar}

* **Descrição**

  Permite ao ator informar um login e uma senha para entrar no sistema. Tal usuário terá acesso ao seu perfil.

* **Atores**

  Somente Usuário não logado.

## \[RF002\] – Logar {#[rf002]-–-logar}

* **Descrição**

  Permite ao ator informar um login e uma senha para entrar no sistema. Tal usuário terá acesso ao seu perfil.

* **Atores**

  Somente Usuário não logado.

  ## \[RF003\] – Recuperar senha  {#[rf003]-–-recuperar-senha}

* **Descrição** 

  O sistema deve permitir que o ator acesse a tela de  recuperação de senha.

* **Atores**

  Somente Usuário não logado.

	\[RF004\] – Logout no sistema 

* **Descrição** 

  Permite ao usuário sair do sistema 

* **Atores**

  Todos os atores, exceto Usuário não logado.

## \[RF005\] – Candidatar-se à atividade {#[rf005]-–-candidatar-se-à-atividade}

* **Descrição**

  O sistema deve permitir que o ator candidate-se a uma nova atividade (TCC, Estágio ou Monitoria).

* **Atores**

  Aluno.

## \[RF006\] – Cancelar candidatura {#[rf006]-–-cancelar-candidatura}

* **Descrição**

  O sistema deve permitir que o ator cancele sua candidatura a uma nova atividade (TCC, Estágio ou Monitoria).

* **Atores**

  Aluno.

  ## \[RF007\] – Visualizar status do processo das atividades {#[rf007]-–-visualizar-status-do-processo-das-atividades}

* **Descrição** 

  O sistema deve permitir que o ator visualize o status de suas atividades acadêmicas.

* **Atores**

  Aluno.

## \[RF008\] – Enviar documentos {#[rf008]-–-enviar-documentos}

* **Descrição**

  O sistema deve permitir que o ator envie documentos obrigatórios por etapa da atividade.

* **Atores**

  Aluno de TCC, estagiário e/ou monitor.

## \[RF009\] – Cancelar envio de documentos {#[rf009]-–-cancelar-envio-de-documentos}

* **Descrição**

  O sistema deve permitir que o ator cancele o envio de documentos obrigatórios por etapa da atividade.

* **Atores**

  Aluno de TCC, estagiário e/ou monitor.

  ## \[RF010\] – Visualizar status dos documentos {#[rf010]-–-visualizar-status-dos-documentos}

* **Descrição** 

  O sistema deve permitir que o ator visualize os documentos enviados e seus status de aprovação.

* **Atores**

  Aluno.

  ## \[RF011\] – Visualizar feedbacks {#[rf011]-–-visualizar-feedbacks}

* **Descrição** 

  O sistema deve permitir que o ator visualize feedbacks e observações feitas por professores e coordenadores.

* **Atores**

  Aluno de TCC, Estagiário e Monitor.

## \[RF012\] – Visualizar lista de alunos {#[rf012]-–-visualizar-lista-de-alunos}

* **Descrição**

  O sistema deve permitir que o ator visualize a lista de alunos sob sua orientação.

* **Atores**

  Professor.

## \[RF013\] – Visualizar o aluno {#[rf013]-–-visualizar-o-aluno}

* **Descrição**

  O sistema deve permitir que o ator visualize as informações específicas de um aluno sob sua orientação.

* **Atores**

  Professor.

## \[RF014\] – Visualizar lista de documentos {#[rf014]-–-visualizar-lista-de-documentos}

* **Descrição**

  O sistema deve permitir que o ator visualize a lista de documentos enviados pelos alunos.

* **Atores**

  Professor.

## \[RF015\] – Visualizar documentos {#[rf015]-–-visualizar-documentos}

* **Descrição**

  O sistema deve permitir que o ator visualize os documentos enviados pelos alunos.

* **Atores**

  Professor.

  ## \[RF016\] – Validar documentos  {#[rf016]-–-validar-documentos}

* **Descrição** 

  O sistema deve permitir que o ator aprove ou rejeite documentos enviados por alunos.

* **Atores**

  Professor.

  ## \[RF017\] – Adicionar feedback  {#[rf017]-–-adicionar-feedback}

* **Descrição** 

  O sistema deve permitir que o ator adicione observações e feedback em documentos e relatórios.

* **Atores**

  Professor.

  ## \[RF018\] – Remover feedback  {#[rf018]-–-remover-feedback}

* **Descrição** 

  O sistema deve permitir que o ator remova observações e feedback em documentos e relatórios.

* **Atores**

  Professor

  ## \[RF019\] – Visualizar histórico  {#[rf019]-–-visualizar-histórico}

* **Descrição** 

  O sistema deve permitir que o ator visualize o histórico completo da atividade de cada aluno.

* **Atores**

  Professor.

  ## \[RF020\] – Registrar andamento da monitoria  {#[rf020]-–-registrar-andamento-da-monitoria}

* **Descrição** 

  O sistema deve permitir que o ator registre o andamento semanal da monitoria.

* **Atores**

  Monitor.

  ## \[RF021\] – Remover andamento da monitoria  {#[rf021]-–-remover-andamento-da-monitoria}

* **Descrição** 

  O sistema deve permitir que o ator remova o andamento semanal da monitoria.

* **Atores**

  Monitor.

## \[RF022\] – Enviar relatórios {#[rf022]-–-enviar-relatórios}

* **Descrição**

  O sistema deve permitir que o ator envie relatórios parciais e finais.

* **Atores**

  Aluno de TCC, Estagiário e Monitor.

## \[RF023\] – Cancelar envio de relatórios {#[rf023]-–-cancelar-envio-de-relatórios}

* **Descrição**

  O sistema deve permitir que o ator cancele o envio de relatórios parciais e finais.

* **Atores**

  Aluno de TCC, Estagiário e Monitor.

  ## \[RF024\] – Cadastrar período de atividades {#[rf024]-–-cadastrar-período-de-atividades}

* **Descrição**  
  Permite ao ator cadastrar os períodos de inscrição e entrega de documentos para cada tipo de atividade (TCC, Estágio, Monitoria).

* **Atores**

  Funcionário administrativo.

  ## \[RF025\] – Editar período de atividades {#[rf025]-–-editar-período-de-atividades}

* **Descrição**  
  Permite ao ator editar os períodos de inscrição e entrega de documentos para cada tipo de atividade (TCC, Estágio, Monitoria).

* **Atores**

  Funcionário administrativo.

  ## \[RF026\] – Editar perfil do usuário {#[rf026]-–-editar-perfil-do-usuário}

* **Descrição**  
  Permite ao ator atualizar dados do seu perfil, como e-mail, telefone e senha.

* **Atores**

   Usuário logado.

  ## \[RF027\] – Reatribuir orientação {#[rf027]-–-reatribuir-orientação}

* **Descrição**  
  Permite ao ator alterar o professor orientador de um aluno em caso de necessidade.

* **Atores**

   Coordenador de Curso.

  ## \[RF028\] – Buscar alunos por filtros {#[rf028]-–-buscar-alunos-por-filtros}

* **Descrição**  
  Permite ao ator filtrar alunos por nome, status da atividade, tipo de atividade (Estágio, TCC, Monitoria e atividade arquivada) e período.

* **Atores**

   Professor.

  ## \[RF029\] – Arquivar atividades finalizadas {#[rf029]-–-arquivar-atividades-finalizadas}

* **Descrição**  
  Permite ao ator arquivar atividades com todos os documentos e relatórios aprovados, encerrando seu fluxo.

* **Atores**

  Professor.

  ## \[RF030\] – Acompanhar prazos e pendências {#[rf030]-–-acompanhar-prazos-e-pendências}

* **Descrição**  
  O sistema deve exibir para o ator as pendências atuais e os prazos para cada etapa da atividade.

* **Atores**

  Aluno e Professor.

  ## \[RF031\] – Validar a elegibilidade do aluno {#[rf031]-–-validar-a-elegibilidade-do-aluno}

* **Descrição**  
  O sistema deve permitir que o ator marque o aluno como elegível ou inelegível quando solicitado um registro de atividade conforme às regras de negócio.

* **Atores**

  Coordenador de Curso.

  ## \[RF032\] \- Visualizar lista de relatórios {#[rf032]---visualizar-lista-de-relatórios}

* **Descrição**

  O sistema deve permitir que o ator visualize a lista de relatórios enviados pelos alunos sob sua orientação ou responsabilidade.

* **Atores**

  Professor

  ## \[RF033\] \- Visualizar relatórios {#[rf033]---visualizar-relatórios}

* **Descrição**

  O sistema deve permitir que o ator visualize o conteúdo dos relatórios enviados pelos alunos. 

* **Atores**

  Professor

  ## \[RF034\] – Obter metadados do documento  {#[rf034]-–-obter-metadados-do-documento}

* **Descrição**

  O sistema deve permitir que o ator obtenha os metadados do documento enviado pelos alunos.

* **Atores**

  Professor.

  ## \[RF035\] – Obter metadados do relatório {#[rf035]-–-obter-metadados-do-relatório}

* **Descrição**

  O sistema deve permitir que o ator obtenha os metadados do relatório enviado pelos alunos.

* **Atores**

  Professor.

	

# 6\. Requisitos não Funcionais {#6.-requisitos-não-funcionais}

| Tipo | Descrição | Prioridade |
| ----- | ----- | ----- |
| **Usabilidade** | O sistema deve ser intuitivo e fácil de navegar, com menus auto explicativos e interface amigável. | Alta |
| **Desempenho** | O sistema deve responder às interações do usuário em até 2 segundos e suportar até 1000 usuários simultâneos. | Alta |
| **Segurança** | Os dados devem ser armazenados de forma segura, com acesso restrito, criptografia e backups periódicos. | Alta |
| **Interface** | O sistema deve ser compatível com navegadores modernos (Chrome, Firefox, Edge) e dispositivos móveis. | Alta |
| **Escalabilidade** | Deve permitir futura integração com o sistema acadêmico oficial da instituição sem necessidade de reestruturação. | Média |
| **Manutenibilidade** | O código-fonte deve ser documentado e modular para facilitar futuras manutenções e atualizações. | Alta |

# 7\. Diagrama de Casos de Uso {#7.-diagrama-de-casos-de-uso}

# 8\. Referências   {#8.-referências}

* Documento de Visão e Requisitos \- [https://quatinetwork.wordpress.com/wp-content/uploads/2012/03/exemplo\_visao.pdf](https://quatinetwork.wordpress.com/wp-content/uploads/2012/03/exemplo_visao.pdf)  
* Documento de Requisitos \- [https://www.cin.ufpe.br/\~if716/projetos/2011\_1/Projeto2\_GerenciadorChamados\_lazs.pdf](https://www.cin.ufpe.br/~if716/projetos/2011_1/Projeto2_GerenciadorChamados_lazs.pdf)  
  

[image1]: <data:image/png;base64,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HXTr1i1xEmRPAGvWrHEnAXVBbSZpx2H06NFmvu7du9NmALQICVMrs4H/qaeecicVpPnatWtnlrn88svdyUCu6ZjXsa82UE6bSZpgAUAxJEytaMGCBakCefSkAdQT21m44oor3EklldsxAQAXCVMraelHBVpOy2s9QD2ItplyqY3RZgC0BAlTK7E93rQ3o2o5u464G1+BrIt+4aESbQYAykXCVGP6CvTAgQNN0D7ggAPcyWXRV6vtCaDYV6uBrLM/qaHS0p/UiP58B20GQDlImGpMT1LXPu/UqVOwdOlSd3LZtB6tjye0I6+ibaal1OZoMwDSIGGqIT2ywfaUK0mPTNE6tX4gT2ybqfRjgWw7pM0ASIqEqYa+//3vmyC95557upNa5N133zXrHTZsWLBt2zZ3MpBJOpZtm9ExXkl77LFH2GYAIAkSphp57rnnTIC+8MIL3UkVccEFF5j1t2/f3p0EZJKO5Vq0meeff96dBADNkDDVwEcffRTst99+Jjh//vnn7uSK0Hq1fhVtD8gyHcP2eK52m+nbty9tBkAsEqYasIH/tttucydV1K233hpuS8+nA7LoD3/4Q6u0GQAohYSpBsaPH1+zgKxtqdBjRlbp2LXHcS2obdZqWwCyi4QJAAAgBgkTAABADBKmMuh5VGme+wagNP2EgNpWpX8+AAAqJVcJk+5D+Od//ufw9aeffmp+82jy5MlfztQC2lc77bSTO7qJpL+xpPn23nvvZuOi7/XQQw8NfvjDHwb3339/cOCBB345YxGXX365Waa16P0PHTrUHY2ccI/tSravuXPnmrb11FNPuZNCat/HHXecO7oZH9oBgPzJVcI0YsSIJsHqk08+MUnOOeecE5krnQ8++CC477773NHNzJgxwx1VkN6Xyu9///sm4+x7VY/773//uxnWPO+99144XzG1vLm8EG173333dUcjJ9xjq5Lt6+KLL3ZHNTN//vzgnnvucUc340M7AJA/dZcwvfzyy+YH6/74xz8Gn332WTj+zjvvDBYsWNDktfX+++8HN910U3DppZcGN9xwQzj+4YcfDpYtWxa88MILwaxZs0yPO7qcvPHGG+aH96699tom423CpF8c/vDDD8Nx0feqbar3rm2+9dZb4XiZNm2aWa+2byU5URRaTrQvLrroomD69OnB8uXLm/3/eh/6/6PvQw8v1deytYwSOjdhKva/I5vcY6tQ+5o6dWowZcoU076sxx57rMnx9Oc//9kUyx5f7nGuZXScXnLJJaZtqX1qXVE6nnV8VasdPPjgg+G0ctpBFO0AyIe6Sph22GEH8/rRRx8Ndt111yaBTcNaPvpadKVHw3q6+TXXXBN069YtOOqoo8y0AQMGmGna5rhx45osZ4dVFCyPOOKIZtOOPPJI87ddu3bhOL1XbVNPVdc2b7zxRrNNu+x1111nhvWRg9ZrtyGlThSlljvppJPM8MSJE4Prr7++yTT7dHe9D/3/Grb/v51PyxxyyCFm2CZMdnvR/z3JVQT4yz22ou1LyYTal5IJJfpqX6eeeqqZ7/DDD2+yrI4fewxFj6/ocS72+LKPL1H71Lokejy7x1e57cAuV6gd7L///mZaoXZg2fcZbQfutEIxAEC2NOSpAY8cObJJwrRp0yYToP7zP//TvLbPj1I57bTTgieeeCKcV+MKJUzyzjvvmB7kt771raBNmzbBPvvsY8YrYRoyZEg4n9jldNVJw7fcckuTaQ888EA4rITpqquuMsMzZ840f6O9dW3zrLPOMtu067Xv35o3b1643lInilLLudNOPPHEJq/1/+t96P/XeP3/zzzzjBm+4447wvn0WglTsf+92HtDNrj1F21fugJk25eOD7Uvq1TCJPb4ih7nouFo+4omTO7xVK12YBMmcduBFGsHUqwd2BgAIFsaigWWLBo9enSw2267ha/t5XH7LKpXXnklGD58eBgYo/+7ho855pgmry37TCvd0KwkSY85EQ2PGjUqnE/sco8//rgZ1n0X0Wlz5swJh5Uw6fEMBx10UNC9e3czziZMV155pXndsWPH8EqWXS763hYuXBiut5wTRXQ5d5puNLev9T70/+t96P/XeP3/9v+79957w+X0WglTsf+92HtDNrj1V6h9tW3bNqzr888/34x3EyYd9zZhih5f0eNcNBxtX6USpmq1A5swFWoHUqwdRKe57cDGAADZ0lAssGTR7NmzTUBSQFaP1wZqe2/SN7/5zWDHHXc0w7/+9a/NtPXr15vXGu7Zs6cZXrRoURj07r77bjOsh+fq/oaBAwc2SZh0GT8quj81bK94rV692rzesmVLOE3vMzqvihKm6DZF27TrPeCAA8zwihUrzGv7jDqt154oXnzxxSZFX9UutZwSNg0/+eST5qMV+16i70v0/2tYy27dutUMa72ijzn12n4kp/Hu//61r33NvEY2qQ51zOqY0r2A0fb1pz/9ybQvJU0SbV+68qvhDRs2mLalj+7cj3UlepzbadH2FU2Yosezji8dkzq+0rQDu1yhdmATpuj7tO1AirUDS8NuO7AxAEC2NEQbd9bp5ksb2KJF9wRJr169zOtTTjkl6NKlS7PApqL7JdSLtNNWrlxphvUxgw22uhokcQmT7k3S6379+pl1qocanS+aMClZ0zglTNqmTira5tlnnx2+N2lsbDTr1bq0Xo2367UnCrfoY79Sy+ljCftxiMpee+0Vbs/e96X34f7/dv6DDz44nM8mTNqeXkf/90ceecRMQzbZhCZavvvd75r2pcRI7UvHxtixY037sldsr7766vC40rEQvQ8wenzZdVoaLpYwRY9n217t8VVuO7DLFWoHNmEq1A4sO3+0HVilYgCAbGmINu680NWl559/3iRQhai3WehZa/rmy8aNG93R5l4NLZOWetXqXZZL21y1apU72li3bp1Zb7kKLaevaj/77LPha/ceJv3/xd6H9qO9SldI2v8dflLbevXVV803yAq1L11FWrJkScH2pfGFlDq+4uh4TnN8JW0H0U5NqfdJOwDyL5cJE8pj7x3RzyToK9D6AUGOC2TN4sWLzVWctAq1g//+7/92ZwNQp0iYYOgXlr/3ve+Zjzwuu+yyYO3ate4sgNd69OhhEp6//vWv7qTE3HYAABYJE4BcUCzTY1F0LxUAVBoJE4DM049C2m/D6qO0Dh06OHMAQMuQMAHItKVLlwZf+cpXwtf217wBoJJImABkmn5b7eSTT24yTs+c43e/AFQSCROATNPHb6+99po72vzqOABUCgkTgMz6l3/5l+Dtt992RxtXXHFFcOaZZ7qjASAVEiYAmVXqKtInn3xiflm70I9oAkC5SJgAZNJPf/pT81DcUvSwbR5HAqASSJgAZJKe6abHlZSybNkyEiYAFUHCBCBz+vbtG+yyyy7m23BxZe7cuUHXrl2DLVu2uKsBgMRImABkjuJWueU73/mOuxoASIyECUAu6BtxxDMA1ULCBCAXSJgAVBMJE4BcIGECUE0kTABygYQJQDWRMAHIBRImANVEwgQgF0iYAFQTCROAXCBhAlBNJEwAcoGECUA1kTAByAUSJgDVRMIEZMSqVauCqVOnNnv0B2V7GTZs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vPDC8Dhq06aNiRlx0xRLNE5xRH/1Ud/bb78dztuzZ0/z1yZMa9eubXK82vvobKy061Oxce7pp58OunTpEo7v3LmzGS/f/OY3m23L0nt2Y6Cl14qB+hsXA4877rhwHfrW53333WfG61jWMW1pumKxuDH2V7/6ldlvdj37779/8Oabb5p5C71PG6uBammINhYf2CAwZsyYsCHr77//+7+bvzZhuu6668xrNZwjjjjCDF988cVN1vGb3/wm+NGPfmSGJ06caKbZE9CUKVOCvn37msZ88sknN1nnoYce2mydNijpxDlu3DgzrjXZhDK6TyyNa42T7Lx580zZb7/9zHuwr5csWRLsvPPOZtwNN9xgeuvf/e53zWt93Cpub96dXglan5Jn+75siVOJK5HRK5uWPbZKKbQcakPHyxlnnOGODkXjRTQ5ipsWjSXDhg0z42wicv311weHHHKIGbYJ09FHHx107do1uPLKK00S9OMf/9iMt3FOHQ/FOg3bOGd/Of7GG28MrrnmmnDbYt9LdFvutGhcdafpPcfFQM2nZOeXv/ylGVb7l7iESa9tjN1hhx3M60cffTT85uipp54aLue+zyTtCWiJhmiD8IENAq+++mrYWPTXnlA1/YUXXjDDt9xyS7icbUB2HdH7DDR+8ODBZjjaY4+eCOPWqcbs9jZbk96XEhPbA3On2f+xVIAqdiWuUO+4nN7bwQcfXPA9ufvP9tSlWG++kvQevvrVr7qjQ4V6s9ErkWeeeaaZL9pzV9ExKuvXrw/HaTv/9m//ZtYj0eOuVO9fr6O9+OhyLa0XlEf72CYghdh6sJR86/UDDzxQcppNDKxnnnnGvL7jjjvCcXqthOnWW281w+ecc47p5J111lnmteKVjZWWjhUb5+Sdd94x8+vWBjtfsW1JsRio92yH3TZayOLFi828t912mzupZDxyY+wee+xhpqvss88+wRNPPGHGF3uf0X0BVEODbwdZNAiowaiH1qdPH/Na4zX98ccfN8PqfVvRBqN5vv3tbzeZpvVIsYQpbp1qzKNGjQqntaa33nrLvK/LLrvM/J8a/vzzz8Ppep00YdJr90pcqSttSbgJkz5y0OtivfW46ZWibbRr184kMdEi77//vpnu9majVyJ/97vfmaRF05SQq+ferVu3cH+edNJJJonRPtS+03yFEqZo71/LR/eVhlVsLz66XKGrFuXUC8qjqzpHHnlkk3EzZ8409SC2rqyFCxea14V+sys6zU2YbOy59957w3F6rYRJ27PripaHHnqoWcKk+GTjnK5GtW/fPujYsaP56NfOV2xb0WluDLQ/Q6LhJDFwwYIFZt67777bnWSO5WOOOSZ8rfmiCVN0/a+88kr4P9py/vnnF32f0X0BVEODbwdZNAjo4xsN6wQmGrYfPx1wwAFhsrN69Woz7Wtf+1q4jmig07RCCZOuGOiEtXXrVvParnPFihXN1qnGrBOiD3RlaeDAgea+B10R6tChQ5OP5fS+kyZMha7EucEn2jtOwk2Y1q1bZ14X663HTa8UbUNX0fQbR9Ein376afh/R3uz4n4kp567ev7quStB0vy6z0nLRnvuJ554YsGESWzv371CqOFoLzu6XEvrBeV57rnnzP5VwqzjQx8VR+tA8ULDihdiP4rWVb9S09yESfGnV69eZhmxV9WVMOkLAUrW7cdwl156qbldYfPmzSUTpuj7/Oyzz8JhbUvD7rYsDbtx1V7F1HDSGKh5+/XrFw7bbYwcOdLcN7Vhw4Zg0aJFZnw0YYquX/da6b5GK7qeQu/TxmqgWhqijcUH0SCgZEDDK1euNK81bBMD+40VNUr1otSbeuSRR8J1JEmYdPVA0xSsxK7T9syi63Qbc2t57LHHwsARLboB0tLraMJUrEdX7EqcXacV7R0n4SZMNki7vXX11N944w0zvVhvXtMrRe+h1EdyhXqz4iZMOi40XT13HRc6Gdpe9Z/+9KdwPj3apFDCFO39uydPDUd72aUSpnLrBeWLfkxri45vUbzQFUvVpeKQpmk4bppb5zJ9+vRw3fbeHXsPk/2Ch+430vuxHw2XSpjsOnQztE3erOj/Yeez9J71OhpXo8sljYF2G1//+tfD9y5XX321ea0v8Wj9Gi6WMCkua/opp5wS3jpgY1mh92ljNVAtDdHGkkXqpaiHkdby5ctNidIVj5ass5rsN8l0hSJaNM5+LKdhe5K1PTpxe3TFEsto71j7QQmBem9J75dxEyaxAU4nEvXWbbC/5JJLzHS3N+9OrwStb9dddw1efPHFJkX7TYlOsd5s9EqkPmbQeL1f9dx1pU/7R/TzFz169AiefPLJYPLkyWa+QglTdN1aPrqvNBw9aUSXK3TVopx6QXpqO8WeIah4oemFlJrm+uijj8x9cIWoTbz00ktl/dL8pk2bglWrVrmjjVLbkpbGVdHH10uXLnVHm1sK9EWQpNRGi81fifcJJNXgntgQTw3YnvTcoo/Jqknb0EnfpStM9uqb5rEnWQVa9Up1WV/3PGlaXMIk9oqJihKBchRKmERfobfr1I3OuizvTrfLarrtSVeKW1e26LeQJHqFST1a+8vO9pL/sccea17bb/zpo7PZs2c3+V+1r9Tj1Udz+jmFAw880IyPJj66d8muwy6vq0Wi4WIJk7SkXoBKac0YCLSWhmiwRzIKCPrWSqES/eaXL9SjS/N7RtW40mZ73Lo6U0zc9Goq1pvVVUh7r5t67prPpa//6/+zdA+T+zGjVar3H6ecqxZANWQtBgKVQMKExOhVlhb9dpQtf/vb39zZKo56AYDqa1BQBZKgVxlv0qRJwfe+9z1zc6o+Aq0F6gUAqo+ECQAAIAYJEwAAQAwSJgAAgBgkTAAAADFImAAAAGKQMAEAAMQgYQIAAIhBwgQAABCDhAkAACAGCRMAAEAMEiYAAIAYJEwAAAAxSJgAAABikDABAADEIGECAACIQcIEAAAQg4QJAAAgBgkTAABADBImAACAGCRMAAAAMUiYAAAAYpAwAQAAxCBhAgAAiEHCBAAAEIOECQAAIAYJEwAAQAwSJgAAgBgkTAAAADH+H5GeIPjzimlqAAAAAElFTkSuQmCC>