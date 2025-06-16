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

**[1\. Introdução	4](#introdução)**

[1.1. Escopo e Alinhamento Estratégico	4](#escopo-e-alinhamento-estratégico)

[1.2. Glossário	4](#glossário)

[**2\. Visão Geral do Produto	5**](#2.-visão-geral-do-produto)

[2.1. Perspectivas do produto	5](#2.1.-perspectivas-do-produto)

[2.2. Regras de negócio	5](#2.2.-regras-de-negócio)

[2.3. Descrição dos atores do sistema	7](#2.3.-descrição-dos-atores-do-sistema)

[**3\. Esquema de Usuários	8**](#3.-esquema-de-usuários)

[**4\. Objetivos de Negócio	9**](#4.-objetivos-de-negócio)

[**5\. Requisitos Funcionais (Casos de Uso)	10**](#5.-requisitos-funcionais-\(casos-de-uso\))

[\[RF001\] – Cadastrar	10](#[rf001]-–-cadastrar)

[\[RF002\] – Logar	10](#[rf002]-–-logar)

[\[RF003\] – Recuperar senha	10](#[rf003]-–-recuperar-senha)

[\[RF004\] – Logout no sistema	10](#[rf004]-–-logout-no-sistema)

[\[RF005\] – Candidatar-se à atividade	11](#[rf005]-–-candidatar-se-à-atividade)

[\[RF006\] – Cancelar candidatura	11](#[rf006]-–-cancelar-candidatura)

[\[RF007\] – Enviar documentos	11](#[rf007]-–-enviar-documentos)

[\[RF008\] – Cancelar envio de documentos	11](#[rf008]-–-cancelar-envio-de-documentos)

[\[RF009\] – Visualizar status dos documentos	12](#[rf009]-–-visualizar-status-dos-documentos)

[\[RF010\] – Visualizar feedbacks	12](#[rf010]-–-visualizar-feedbacks)

[\[RF011\] – Visualizar o aluno	12](#[rf011]-–-visualizar-o-aluno)

[\[RF012\] – Visualizar documentos	12](#[rf012]-–-visualizar-documentos)

[\[RF013\] – Validar documentos	13](#[rf013]-–-validar-documentos)

[\[RF014\] – Adicionar feedback	13](#[rf014]-–-adicionar-feedback)

[\[RF015\] – Remover feedback	13](#[rf015]-–-remover-feedback)

[\[RF016\] – Visualizar histórico	13](#[rf016]-–-visualizar-histórico)

[\[RF017\] – Configurar formulário de atividades	14](#[rf017]-–-configurar-formulário-de-atividades)

[\[RF018\] – Editar perfil do usuário	14](#[rf018]-–-editar-perfil-do-usuário)

[\[RF019\] – Reatribuir orientação	14](#[rf019]-–-reatribuir-orientação)

[\[RF020\] – Buscar atividade por filtros	14](#[rf020]-–-buscar-atividade-por-filtros)

[\[RF021\] – Arquivar atividades finalizadas	14](#[rf021]-–-arquivar-atividades-finalizadas)

[\[RF022\] – Validar a elegibilidade do aluno	15](#[rf022]-–-validar-a-elegibilidade-do-aluno)

[\[RF023\] – Visualizar lista de atividades	15](#[rf023]-–-visualizar-lista-de-atividades)

[\[RF024\] – Visualizar atividade	15](#[rf024]-–-visualizar-atividade)

[\[RF025\] – Verificar permissões de acesso	15](#[rf025]-–-verificar-permissões-de-acesso)

[\[RF026\] \- Visualizar lista de candidaturas	16](#[rf026]---visualizar-lista-de-candidaturas)

[\[RF027\] \- Visualizar candidatura	16](#[rf027]---visualizar-candidatura)

[\[RF028\] \- Validar candidaturas de atividades	16](#[rf028]---validar-candidaturas-de-atividades)

[\[RF029\] \- Visualizar status do processo das candidaturas	16](#[rf029]---visualizar-status-do-processo-das-candidaturas)

[\[RF030\] \- Cancelar atividade	16](#[rf030]---cancelar-atividade)

[\[RF031\] \- Visualizar perfil do usuário	17](#[rf031]---visualizar-perfil-do-usuário)

[**6\. Requisitos não Funcionais	17**](#6.-requisitos-não-funcionais)

[**7\. Diagrama de Casos de Uso	17**](#7.-diagrama-de-casos-de-uso)

[**8\. Referências	19**](#8.-referências)

1. # Introdução {#introdução}

Este projeto visa desenvolver um sistema para auxiliar alunos e professores no gerenciamento das atividades obrigatórias e complementares do curso, como TCC, Estágio e Monitoria. O sistema busca organizar documentos, etapas de aprovação e relatórios, facilitando o acompanhamento e cumprimento dos requisitos dessas atividades. Para os alunos será possível registrar e acompanhar o progresso das atividades acadêmicas (TCC, Estágio, Monitoria), enquanto professores e coordenadores possam realizar a validação e acompanhamento de documentos e relatórios.

1. ## Escopo e Alinhamento Estratégico {#escopo-e-alinhamento-estratégico}

   O Sistema de Gerenciamento de Atividades Acadêmicas (TCC, Estágio e Monitoria) é um projeto realizado para a disciplina de Análise e Desenvolvimento de Software.

   **O sistema permitirá:**

* Gerenciamento de usuários por perfil (Usuário não logado, Usuário logado, Aluno, Orientando, Professor, Coordenador de curso e Funcionário administrativo);  
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
| Aluno | Este ator representa um estudante regularmente matriculado, que pode se candidatar em uma ou mais atividades (TCC, Estágio, Monitoria). | Candidatar-se em TCC, estágio e/ou monitoria, de acordo com regras de negócio. Acompanhar candidaturas efetuadas. |
| Orientando | Este ator representa um estudante que está envolvido em uma ou mais atividades (TCC, Estágio, Monitoria). | Enviar documentos (Termos de compromisso, relatórios, projetos e andamento da monitoria). Acompanhar validações do professor orientador. |
| Professor  | Ator que representa um docente responsável por acompanhar o desenvolvimento de uma ou mais atividades (TCC, Estágio ou Monitoria) dos aorientandos. | Validar registros e documentos submetidos por orientandos. Fornecer feedbacks das atividades do seu orientando. Acompanhar progresso e status das atividades orientadas. |
| Coordenador de curso | Ator que representa um docente responsável por acompanhar e autorizar a finalização das atividades acadêmicas dos alunos. | Validar a elegibilidade de Alunos para/com as atividades. |
| Funcionário administrativo | Ator com funções operacionais e de apoio ao sistema, como gestão de prazos e organização documental. | Validar informações cadastrais dos usuários. Configurar regras e prazos institucionais. |

# 3\. Esquema de Usuários {#3.-esquema-de-usuários}

![][image1]

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

  Usuário não logado.

## \[RF002\] – Logar {#[rf002]-–-logar}

* **Descrição**

  Permite ao ator informar um login e uma senha para entrar no sistema. Tal usuário terá acesso ao seu perfil.

* **Atores**

  Usuário não logado.

  ## \[RF003\] – Recuperar senha  {#[rf003]-–-recuperar-senha}

* **Descrição** 

  O sistema deve permitir que o ator acesse a tela de  recuperação de senha.

* **Atores**

  Usuário não logado.

  ## \[RF004\] – Logout no sistema  {#[rf004]-–-logout-no-sistema}

* **Descrição** 

  Permite ao usuário sair do sistema 

* **Atores**

  Usuário logado.

## \[RF005\] – Candidatar-se à atividade  {#[rf005]-–-candidatar-se-à-atividade}

* **Descrição**

  O sistema deve permitir que o ator candidate-se a uma nova atividade (TCC, Estágio ou Monitoria).

* **Atores**

  Aluno.

## \[RF006\] – Cancelar candidatura {#[rf006]-–-cancelar-candidatura}

* **Descrição**

  O sistema deve permitir que o ator cancele sua candidatura a uma nova atividade (TCC, Estágio ou Monitoria).

* **Atores**

  Aluno.

## \[RF007\] – Enviar documentos {#[rf007]-–-enviar-documentos}

* **Descrição**

  O sistema deve permitir que o ator envie documentos obrigatórios por etapa da atividade.

* **Atores**

  Orientando.

## \[RF008\] – Cancelar envio de documentos {#[rf008]-–-cancelar-envio-de-documentos}

* **Descrição**

  O sistema deve permitir que o ator cancele o envio de documentos obrigatórios por etapa da atividade.

* **Atores**

  Orientando.

  ## \[RF009\] – Visualizar status dos documentos {#[rf009]-–-visualizar-status-dos-documentos}

* **Descrição** 

  O sistema deve permitir que o ator visualize os documentos enviados e seus status de aprovação.

* **Atores**

  Orientando.

  ## \[RF010\] – Visualizar feedbacks {#[rf010]-–-visualizar-feedbacks}

* **Descrição** 

  O sistema deve permitir que o ator visualize feedbacks e observações feitas por professores e coordenadores.

* **Atores**

  Orientando.

## \[RF011\] – Visualizar o aluno {#[rf011]-–-visualizar-o-aluno}

* **Descrição**

  O sistema deve permitir que o ator visualize as informações específicas de um aluno sob sua orientação em uma atividade específica.

* **Atores**

  Professor.

## \[RF012\] – Visualizar documentos {#[rf012]-–-visualizar-documentos}

* **Descrição**

  O sistema deve permitir que o ator visualize os documentos enviados pelos orientandos.

* **Atores**

  Professor e Orientando.

  ## \[RF013\] – Validar documentos  {#[rf013]-–-validar-documentos}

* **Descrição** 

  O sistema deve permitir que o ator aprove ou rejeite documentos enviados por orientandos.

* **Atores**

  Professor.

  ## \[RF014\] – Adicionar feedback  {#[rf014]-–-adicionar-feedback}

* **Descrição** 

  O sistema deve permitir que o ator adicione observações e feedback em documentos.

* **Atores**

  Professor.

  ## \[RF015\] – Remover feedback  {#[rf015]-–-remover-feedback}

* **Descrição** 

  O sistema deve permitir que o ator remova observações e feedback em documento.

* **Atores**

  Professor

  ## \[RF016\] – Visualizar histórico  {#[rf016]-–-visualizar-histórico}

* **Descrição**  
  Permite ao ator consultar o histórico das atividades acadêmicas (TCC, Estágio ou Monitoria) participadas ou orientadas que já foram concluídas.   
* **Atores** 

  Professor e Orientando.

  ## \[RF017\] – Configurar formulário de atividades {#[rf017]-–-configurar-formulário-de-atividades}

* **Descrição**  
  Permite ao ator configurar os formulários de candidatura de cada tipo de atividade (TCC, Estágio, Monitoria).

* **Atores**

  Funcionário administrativo.

  ## \[RF018\] – Editar perfil do usuário {#[rf018]-–-editar-perfil-do-usuário}

* **Descrição**  
  Permite ao ator atualizar dados do seu perfil, como foto, telefone e senha.

* **Atores**

   Usuário logado.

  ## \[RF019\] – Reatribuir orientação {#[rf019]-–-reatribuir-orientação}

* **Descrição**  
  Permite ao ator alterar o professor orientador de um aluno em caso de necessidade.

* **Atores**

   Coordenador de Curso.

  ## \[RF020\] – Buscar atividade por filtros {#[rf020]-–-buscar-atividade-por-filtros}

* **Descrição**  
  Permite ao ator filtrar atividades por aluno, status da atividade, tipo de atividade (Estágio, TCC, Monitoria) e período.

* **Atores**

   Professor, Orientando e Coordenador de Curso.

  ## \[RF021\] – Arquivar atividades finalizadas {#[rf021]-–-arquivar-atividades-finalizadas}

* **Descrição**  
  Permite ao ator arquivar atividades com todos os documentos e relatórios aprovados, encerrando seu fluxo.

* **Atores**

  Professor.

  ## \[RF022\] – Validar a elegibilidade do aluno {#[rf022]-–-validar-a-elegibilidade-do-aluno}

* **Descrição**  
  O sistema deve permitir que o ator marque o aluno como elegível ou inelegível quando solicitado um registro de atividade conforme às regras de negócio.

* **Atores**

  Coordenador de Curso.

  ## \[RF023\] – Visualizar lista de atividades {#[rf023]-–-visualizar-lista-de-atividades}

* **Descrição**

  O sistema deve permitir que o ator visualize a lista de atividades que ele orienta ou participa.

* **Atores**

  Professor e Orientando.


  ## \[RF024\] – Visualizar atividade {#[rf024]-–-visualizar-atividade}

* **Descrição**

  O sistema deve permitir que o ator visualize a atividade que ele orienta ou participa.

* **Atores**

  Professor e Orientando.


  ## \[RF025\] – Verificar permissões de acesso {#[rf025]-–-verificar-permissões-de-acesso}

* **Descrição**

  O sistema deve verificar qual ator está fazendo a solicitação e permitir que ele acesse o recurso solicitado para o seu perfil de ator.

* **Atores**

  Sem atores.


  ## \[RF026\] \- Visualizar lista de candidaturas {#[rf026]---visualizar-lista-de-candidaturas}

* **Descrição**  
  Permite que o ator visualize a lista de candidaturas à uma atividade enviadas ou recebidas.  
* **Atores** 

  Professor e Aluno.

  ## \[RF027\] \- Visualizar candidatura {#[rf027]---visualizar-candidatura}

* **Descrição**  
  Permite que o ator visualize a candidatura à uma atividade.  
* **Atores** 

  Professor e Aluno.

  ## \[RF028\] \- Validar candidaturas de atividades {#[rf028]---validar-candidaturas-de-atividades}

* **Descrição**

  Permite que o ator aprove ou rejeite solicitações de candidaturas enviadas pelos alunos.

* **Atores**

  Professor


  ## \[RF029\] \- Visualizar status do processo das candidaturas {#[rf029]---visualizar-status-do-processo-das-candidaturas}

* **Descrição**  
  Permite que o ator visualize o status do processo das suas candidaturas.  
* **Atores** 

  Aluno


  ## \[RF030\] \- Cancelar atividade {#[rf030]---cancelar-atividade}

* **Descrição**  
  Permite que o ator cancele uma atividade que ele orienta.  
* **Atores** 

  Professor


  ## \[RF031\] \- Visualizar perfil do usuário {#[rf031]---visualizar-perfil-do-usuário}

* **Descrição**  
  Permite que o ator visualize o seu perfil.  
* **Atores** 

  Usuário Logado

  ## 

	

# 6\. Requisitos não Funcionais {#6.-requisitos-não-funcionais}

| Tipo | Descrição | Prioridade |
| ----- | ----- | ----- |
| **Usabilidade** | O sistema deve ser intuitivo e fácil de navegar, com menus auto explicativos e interface amigável. | Alta |
| **Desempenho** | O sistema deve responder às interações do usuário em até 2 segundos e suportar até 1000 usuários simultâneos. | Alta |
| **Segurança** | Os dados devem ser armazenados de forma segura, com acesso restrito, criptografia e backups periódicos. | Alta |
| **Interface** | O sistema deve ser compatível com navegadores modernos (Chrome, Firefox, Edge) e dispositivos móveis. | Alta |
| **Escalabilidade** | Deve permitir futura integração com o sistema acadêmico oficial da instituição sem necessidade de reestruturação. | Média |
| **Manutenibilidade** | O código-fonte deve ser documentado e modular para facilitar futuras manutenções e atualizações. | Alta |

# 

# 7\. Diagrama de Casos de Uso {#7.-diagrama-de-casos-de-uso}

![][image2]

# 8\. Referências   {#8.-referências}

* Documento de Visão e Requisitos \- [https://quatinetwork.wordpress.com/wp-content/uploads/2012/03/exemplo\_visao.pdf](https://quatinetwork.wordpress.com/wp-content/uploads/2012/03/exemplo_visao.pdf)  
* Documento de Requisitos \- [https://www.cin.ufpe.br/\~if716/projetos/2011\_1/Projeto2\_GerenciadorChamados\_lazs.pdf](https://www.cin.ufpe.br/~if716/projetos/2011_1/Projeto2_GerenciadorChamados_lazs.pdf)




[image1]: <data:image/png;base64,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CCUJyrG2te3999+v22/X4zFgTTFs2LAwZp944om6/YxnAB5lfXAjlCTouw022CC07XXXXZceCq699tpw3OLsZXagyubOnRvG66GHHpoeChjPAHqj1BpuhJIEffPxxx+Hdj355JPTQ3VOOumkEPflL385PQRUio1Te9P4G2+8kR6qYTwDaEapNdwIJQl0t9xyS3hD4vrrr58eamjs2LGhDxYsWJAeAgbcihUrsl133VVeJxjPABpR1hA3QkkCzYcffhjas69teuqpp4bb2O2BKunp6Qlj89lnn00PNcV4BpBSnhfdCCUJfP39H773nheg0w455JAwJu39K33FeAaQp9QaboSSBL711lsvtOWf/vSn9JDEbme3tzzAQLvsssvCePzsZz+bvfPOO+lhF+MZQJ5Sa7gRShL07qijjgrtuPfee6eH+sRub3ksHzBQyv5rM8V4BhAp64kboSRBc+uss05ow1ad6TM9My7Qafam8fHjx2cvvfRSeqjPGM8AjFJruBFKEjRmL5W34i/RVMxZ5qV4oD/sbLU29uzTbq3CeAagPE+6EUoSNGZtN2nSpF7PTVGG5bO89A066aKLLgpjbptttkkP9Ut+PF988cXpYQBdQHk+cyOUJGhsxIgR6a6Wand+IM8KlrXXXjvd3TI2ni+55JJ0N4AuoNQaboSSBAAAoCyl1nAjlCQAAABlKbWGG6EkqZpGj7nRvr7qLUdvxyKLufDCCwv7ouOPPz58v9DixYtzEc0p99lKnb4/9I31T9pHjfb1ld3+rLPOSncHSn7veDsMxH0CKE+Zs26EkqRqGj3mRvs6LS7uX/va1+r2ldWf25bR6ftD3zQqHhrt67SBuP+BuE8A5Slz1o1QklRNo8ec33fsscdmm266abbFFltk77//fu14PiZ/+eyzz84mT56cjRs3Lnv++edrx22zLzG0b5/Nxy9dujQ78MADw1k8n3zyydp+iznyyCN7vR9742H+fozlsy+NO+CAAwr5mon3b7fJ23rrrcMbJ+27X5T73m677cL+hQsXFn5He0zp74iBk47hdF9+3J922ml1MfnL8Xp+3B988MF1MflxH+Pz4z4/7tLHlNdsHN18881hrM6cObNurK5cuTI8JhuT9pjiWL311lvDWJ06dWphrNpjajR/AFRHb+tE5EYoSaqm0WNOF+W//e1v2a9+9ats4403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>

[image2]: <data:image/png;base64,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>
