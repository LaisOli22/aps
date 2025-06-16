**Especificações de Casos de Uso**

# **\[UC01\] Cadastrar**

**Fluxo Básico:**

1. O sistema exibe o formulário de cadastro.   
2. O ator informa um login e uma senha.  
3. O sistema valida os dados inseridos (formato, preenchimento, unicidade do login). \[FE01\]  \[FE02\]  
4. O ator confirma o cadastro. \[FA01\]  
5. O sistema salva os dados e exibe uma mensagem de sucesso.

**Fluxos Alternativos:**

**1\. Cancelar Operação:**  
Ocorre quando o ator opta por não concluir o cadastro.Retorna à tela inicial do sistema.

**Fluxos de exceção:**

**1\. Dados inválidos ou incompletos:**  
Ocorre quando o ator deixa campos obrigatórios em branco ou preenche com dados em formato inválido.

**2\. Login já existente:**  
Ocorre quando o login informado já está em uso por outro usuário.

# **\[UC02\] Logar**

**Fluxo Básico:**

1. O sistema exibe o formulário de login.   
2. O ator informa seu login e senha. \[FA01\]  
3. O sistema valida os dados inseridos (formato, preenchimento.) \[FE01\]  
4. O sistema verifica as credenciais.\[FE02\], \[FE03\]  
5. O sistema autentica o ator e redireciona para a área logada.

**Fluxos Alternativos:**

**1\. Cancelar Operação:**  
Ocorre quando o ator opta por não continuar com o login. Retorna à tela inicial do sistema.

**Fluxos de exceção:**

**1\. Dados inválidos ou incompletos:**  
Ocorre quando o ator não preenche os campos obrigatórios ou os preenche com um formato inválido (ex: campo em branco).

**2\. Credenciais incorretas**:  
Ocorre quando o login ou a senha estão incorretos. O sistema exibe uma mensagem de erro e permite nova tentativa.

**3\. Usuário inexistente:**  
Ocorre quando o login informado não está cadastrado no sistema. O sistema informa que o usuário não foi encontrado.

# **\[UC03\]  Recuperar senha**

**Fluxo Básico:**

1. O sistema exibe o formulário de recuperação de senha.   
2. O ator informa seu login (e-mail ou nome de usuário cadastrado). \[FA01\]  
3. O sistema valida o dado inserido (formato, preenchimento). \[FE01\]  
4. O sistema verifica se o login está cadastrado. \[FE02\]  
5. O sistema envia um código de recuperação para o e-mail associado.  
6. O ator insere o código de recuperação no sistema.\[FE03\]  
7. O sistema exibe o formulário para criação de nova senha.  
8. O ator informa e confirma a nova senha.  
9. O sistema valida a nova senha (formato, critérios de segurança). \[FE04\]  
10. O sistema atualiza a senha e exibe uma mensagem de sucesso.

**Fluxos Alternativos:**

**1\. Cancelar Operação**:  
Ocorre quando o ator opta por não continuar o processo de recuperação. Retorna à tela inicial do sistema.

**Fluxos de exceção:**

**1\. Dados inválidos ou incompletos:**  
Ocorre quando o ator não preenche o campo de login ou o preenche com dados em formato inválido.

**2\. Usuário inexistente:**  
Ocorre quando o login informado não está cadastrado no sistema. O sistema informa que o usuário não foi encontrado.  
**3\. Código de recuperação inválido:**  
Ocorre quando o código informado está incorreto. O sistema solicita nova solicitação de recuperação.

**4\. Nova senha inválida:**  
Ocorre quando a nova senha não atende aos critérios mínimos de segurança (ex: comprimento, caracteres especiais). O sistema exibe mensagem de erro e solicita nova senha.

# **\[UC04\] Logout do Sistema**

**Fluxo Básico:**

1. O ator solicita logout do sistema   
2. O sistema encerra a sessão do ator.  
3. O sistema redireciona o ator para a tela de login  
4. O sistema exibe uma mensagem de confirmação de logout bem sucedido.

# **\[UC05\] Candidatar-se à Atividade**

**Pré-Condição:** 

1. A atividade estar disponível para receber as candidaturas   
   

**Fluxo Básico:**

1. O ator seleciona uma atividade desejada.  
2. O sistema exibe os detalhes da atividade, incluindo os editais, e o formulário de candidatura.  
3. O ator preenche as informações solicitadas (ex: justificativa, disponibilidade,e documentos)  
4. O sistema valida os dados inseridos. \[FE01\] \[FE02\]  
5. O ator confirma a candidatura. \[FA01\]  
6. O sistema registra a candidatura e exibe uma mensagem de sucesso.

**Fluxos Alternativos:**

**1\. Cancelar Operação:**  
Ocorre quando o ator opta por não prosseguir com o cancelamento. Retorna ao passo 1\.

**Fluxos de exceção:**

**1\. Dados inválidos ou incompletos:**  
Ocorre quando o ator deixa campos obrigatórios em branco ou preenche com dados em formato inválido.  
**2\. Candidatura duplicada:**  
Ocorre quando o ator tenta se candidatar a uma atividade para a qual já está inscrito.

# **\[UC06\] Cancelar candidatura**

**Pré-Condição:** 

1. O ator deve possuir uma candidatura ativa em alguma atividade (TCC, Estágio ou Monitoria).  
2. O ator acessou a candidatura por meio do caso de uso \[UC27 \- Visualizar Candidatura   
   

**Fluxo Básico:**

1. O ator seleciona a candidatura que deseja cancelar.  
2. O sistema exibe os detalhes da candidatura e a opção de cancelamento.   
3. O ator confirma o cancelamento da candidatura. \[FA01\]  
4. O sistema registra o cancelamento.  
5. O sistema exibe uma mensagem de confirmação de cancelamento bem sucedido.

**Fluxos Alternativos:**

**1\. Cancelar Operação:**  
Ocorre quando o ator opta por não prosseguir com o cancelamento. Retorna ao passo 1\.

# **\[UC07\] Enviar Documentos**

**Pré-condição:**

1. O ator acessou a atividade pelo caso de uso \[UC24\] \- Visualizar atividade.

**Fluxo Básico:**

1. O sistema solicita o upload dos arquivos. \[FA001\]  
2. O ator faz upload dos arquivos  
3. O sistema valida o formato dos arquivos. \[FE001\]  
4. O ator confirma o envio dos arquivos. \[FA001\]  
5. O sistema envia os documentos para o Professor Orientador

**Fluxos Alternativos:**

**1\. Cancelar operação**  
	Ocorre quando o ator deseja cancelar a operação de envio de documentos. O sistema solicitará a confirmação do cancelamento. O caso de uso é encerrado.

**Fluxos de exceção:**

**1\. Formato de arquivo inválido:**  
Ocorre quando os arquivos enviados pelo ator não estão no formato Portable Document Format (PDF). O sistema exibe uma mensagem de erro informando que o formato dos arquivos deve ser PDF. Retorna ao passo 1\.

# **\[UC08\] Cancelar envio de documentos**

**Pré-condição:**

1. O ator acessou a atividade pelo caso de uso \[UC24\] \- Visualizar atividade.  
2.  O ator enviou o documento pelo caso de uso \[UC07\] \- Enviar documentos.

**Fluxo Básico:**

1. O ator seleciona o documento a ser cancelado  
2. O sistema solicita a confirmação do cancelamento  
3. O ator confirma o cancelamento \[FA01\]  
4. O sistema remove os documentos \[FE01\] 

**Fluxos alternativos:**

**1\. Cancelar operação:**  
	Ocorre quando o ator não confirma o cancelamento. A mensagem de confirmação some. Retorna ao passo 1\.

**Fluxos de exceção:**

**1\. Erro de confirmação:**  
	Ocorre quando o sistema não consegue remover os documentos enviados por falha na conexão com o banco de dados. O sistema exibe uma mensagem informando que a ação de cancelamento não foi bem sucedida. Retorna ao passo 1\.

# **\[UC09\] Visualizar status do documento**

**Pré-condição:**

1. O ator acessou a atividade pelo caso de uso \[UC24\] \- Visualizar atividade.   
2. O ator precisa ter enviado um documento com o caso de uso \[UC07\] \- Enviar documento.

**Fluxo Básico:**

1. O sistema exibe o status de validação do documento

# **\[UC10\] Visualizar Feedbacks**

**Pré-condição:**

1. O ator acessou a atividade pelo caso de uso \[UC24\] \- Visualizar atividade.   
2. A atividade deve ter sido validada pelo professor orientador.

**Fluxo Básico:**

1. O ator seleciona o documento cujo feedback será visualizado  
2. O sistema exibe o feedback do documento \[FA01\]   
   

**Fluxos alternativos:**  
**1\. Documento sem feedback:**  
	Ocorre quando o documento foi validado mas não houve feedback associado. O sistema deve mostrar uma mensagem esclarecendo que não houve feedback. Termina o fluxo básico.

# **\[UC11\] Visualizar aluno**

**Pré-condição:**

1. O ator acessou a atividade pelo caso de uso \[UC24\] \- Visualizar atividade.   
2. O aluno deve ser orientado pelo professor.

**Fluxo Básico:**

1. O ator seleciona o aluno a ser visualizado.  
2. O sistema exibe as informações principais do aluno. 

# **\[UC012\] \- Visualizar documentos**

**Pré-condição:**

1. O ator acessou a atividade por meio do caso de uso \[UC24\] \- Visualizar atividade.  
   

**Fluxo Principal:**

1. O ator clica sobre um documento específico. \[FE01\]  
2. O sistema abre o documento em visualização (PDF, DOC, etc.) em uma nova aba ou faz o download.

**Fluxo de exceção:**

**1\. Arquivo corrompido:**  
Caso o arquivo esteja corrompido ou não possa ser aberto, o sistema exibe a mensagem “Não foi possível abrir o documento.” O caso de uso é encerrado.

# **\[UC13\] \- Validar documentos**

**Pré-condição:** 

1. O ator acessou um documento específico de um aluno por meio do caso de uso \[UC012\] \- Visualizar documentos.  
2. O status do documento deve estar pendente.  
   

**Fluxo Principal:**

1. O sistema exibe opções de “Aprovar” ou “Rejeitar”.  
2. O ator seleciona a opção desejada. \[FA01\]\[FE01\]  
3. O sistema pede confirmação da opção escolhida.  
4. O ator confirma a opção escolhida. \[FA02\]  
5. O sistema registra a decisão e altera o status do documento.  
   

**Fluxo Alternativo:**

**1\. Adicionar feedback:**  
Ocorre caso o ator queira comentar, ou inserir um feedback, dessa forma, o processo deve seguir o fluxo do caso de uso \[UC014\] \- Adicionar feedback.

**2\. Cancelar a operação:**  
Ocorre quando o ator não confirma a opção selecionada. A mensagem de confirmação some. Retorna ao passo 1\.

**Fluxo de exceção:**  
**1\. Documento já validado:**  
Ocorre se o ator tentar validar um documento já aprovado/rejeitado, o sistema bloqueia a ação e exibe a mensagem: “Este documento já foi validado”. Retorna ao passo 1 do fluxo principal.

# **\[UC14\] \- Adicionar feedback**

**Pré-condição:** 

1. O ator acessou um documento específico de um aluno por meio do caso de uso \[UC012\] \- Visualizar documentos.  
   

**Fluxo Principal:**

1. O ator acessa o documento enviado por um aluno.  
2. O sistema exibe um campo para comentários.  
3. O ator insere um feedback.  
4. O ator confirma o envio do feedback. \[FE01\]  
5. O sistema salva e anexa o feedback ao documento.  
   

**Fluxo de exceção:**

**1\. Campo em branco:**  
Ocorre se o ator deixar o campo de feedback em branco, o sistema exibe a mensagem: “Insira um comentário antes de enviar”. Retorna ao passo 2 do fluxo principal.

# **\[UC15\] – Remover feedback** 

**Pré-condição:** 

1. O ator acessou um documento específico de um aluno por meio do caso de uso \[UC012\] \- Visualizar documentos.  
2. O feedback desse documento já deve ter sido enviado.  
   

**Fluxo Básico:**

1. O ator seleciona o feedback a ser removido.  
2. O sistema exibe o feedback.  
3. O ator solicita a remoção do feedback.  
4. O sistema solicita a confirmação da remoção.  
5. O ator confirma a remoção. \[FA01\]  
6. O sistema remove o feedback. \[FE01\] 

**Fluxos alternativos:**

**1\. Cancelar operação:**  
Ocorre quando o ator não confirma o cancelamento. A mensagem de confirmação some. Retorna ao passo 1\.

**Fluxos de exceção:**

1\. Falha na remoção:  
Ocorre quando o sistema não consegue remover os feedbacks enviados por falha na conexão com o banco de dados. O sistema exibe uma mensagem informando que a ação de cancelamento não foi bem sucedida. Retorna ao passo 1\.

# **\[UC16\] \- Visualizar histórico**

**Pré-condição:** 

1. As atividades acadêmicas (TCC, Estágio e/ou Monitoria) já devem ter sido arquivadas.  
   

**Pontos de Extensão:** 

- Filtrar documentos por ator


**Fluxo Básico:**

1. O ator solicita a exibição do histórico das atividades finalizadas.  
2. Inclui o caso de uso “Verificar permissões de acesso”  
3. Ponto de extensão: Filtrar histórico por ator  
   

**\[UC016 \- EXT1\] \- Acesso do professor:**

**Estende:** UC016 \- Visualizar histórico.  
**Ponto de Extensão:** Filtrar histórico por ator.  
**Condição:** Ator \= Professor.

**Fluxo de extensão:**

1. O sistema coleta os metadados das atividades das quais o ator foi orientador.  
2. O sistema exibe a lista de atividades orientadas \[FA01\].

**Fluxos alternativos:**

**1\. Nenhuma atividade finalizada:**  
	Ocorre quando não houverem atividades finalizadas nas quais o ator foi orientador. O sistema exibe uma mensagem informando que não houve atividade finalizada. O caso de uso é encerrado.

**\[UC016 \- EXT2\] \- Acesso do Orientando:**

**Estende:** UC016 \- Visualizar histórico.  
**Ponto de Extensão:** Filtrar histórico por ator.  
**Condição:** Ator \= Orientando.

**Fluxo de extensão:**

1. O sistema coleta os metadados das atividades participadas pelo ator.  
2. O sistema exibe a lista das atividades \[FA01\].

**Fluxos alternativos:**

**1\. Nenhuma atividade finalizada:**  
	Ocorre quando não houverem atividades finalizadas nas quais o ator participou. O sistema exibe uma mensagem informando que não houve atividade finalizada. O caso de uso é encerrado.

### **\[UC017\] Configurar Formulário de Atividade**

**Fluxo Básico:**

1. O ator seleciona o tipo de atividade (TCC, Estágio ou Monitoria)  
2. O sistema exibe uma interface para configurar campos, períodos e critérios no formulário  
3. O ator preenche e seleciona as opções desejadas  
4. O sistema valida os dados inseridos \[FE001\]  
5. O ator confirma a configuração \[FA001\]  
6. O sistema salva a estrutura do edital e exibe mensagem de sucesso

**Fluxo Alternativo:**

1. **Cancelar operação:**

Ocorre quando o ator não confirma a opção selecionada. A mensagem de confirmação some. Retorna ao passo 2\.

**Fluxo de Exceção:**

1. **Campos inválidos ou configuração incompleta:**

   Ocorre quando algum dado obrigatório não foi definido. O sistema exibe mensagem de erro e retorna ao passo 2\.

# **\[UC18\] Editar Perfil do Usuário**

**Fluxo Básico:**

1. O ator acessa a área de perfil  
2. O sistema exibe os dados atuais  
3. O ator edita e atualiza foto, telefone ou senha  
4. O sistema valida os dados (ex: formato de e-mail, força da senha) \[FE001\]  
5. O ator confirma a atualização \[FA001\]  
6. O sistema salva os dados e exibe mensagem de confirmação

**Fluxo Alternativo:**

**1\. Cancelar operação:**  
Ocorre quando o ator não confirma a opção selecionada. A mensagem de confirmação some. Retorna ao passo 2\.

**Fluxo de Exceção:**

**1\. Dados inválidos:**  
O sistema exibe erro e impede o envio até que os campos sejam corrigidos. Retorna ao passo 2\.

# **\[UC19\] Reatribuir Orientação**

**Pré-condição:** 

1. O ator acessou a atividade por meio do caso de uso \[UC24\] \- Visualizar atividade.

**Fluxo Básico:**

1. O ator solicita reatribuição da orientação da atividade  
2. O ator escolhe um novo professor orientador \[FE001\]  
3. O sistema solicita confirmação da troca  
4. O ator confirma \[FA001\]  
5. O sistema atualiza o orientador e notifica ambos os envolvidos (Professor e Orientando)

**Fluxo Alternativo:**

**1\. Cancelar operação:**  
Ocorre quando o ator não confirma a opção selecionada. A mensagem de confirmação some. Retorna ao passo 2\.

**Fluxo de Exceção:**

**1\. Professor indisponível:**  
O sistema informa que o novo professor não pode ser atribuído. Retorna ao passo 1\.

# **\[UC20\] Buscar Atividade por Filtros**

**Pré-condição:** 

1. O ator acessou o histórico por meio do caso de uso \[UC16\] \- Visualizar histórico.  
2. O ator acessou a lista de atividades por meio do caso de uso \[UC24\] \- Visualizar lista de atividades, no caso do ator Coordenador de Curso.

**Fluxo Básico:**

1. O ator acessa a funcionalidade de busca.  
2. O sistema exibe os filtros disponíveis (aluno, status, tipo de atividade, período).  
3. O ator seleciona os filtros desejados.  
4. O sistema exibe a lista de atividades correspondentes aos filtros aplicados.

# **\[UC21\] Arquivar Atividades Finalizadas**

**Pré-condição:** 

1. O ator acessou a lista de atividades por meio do caso de uso \[UC23\] \- Visualizar lista de atividades.

**Fluxo Básico:**

1. O ator seleciona a atividade finalizada que deseja arquivar.  
2. O sistema solicita a confirmação do arquivamento.  
3. O ator confirma a ação \[FA001\]  
4. O sistema arquiva a atividade, bloqueando novas interações e alterações.  
5. O sistema exibe uma mensagem de sucesso.  
   

**Fluxo Alternativo:**

1. Cancelar operação:

Ocorre quando o ator não confirma a opção selecionada. A mensagem de confirmação some. Retorna ao passo 1\.

# **\[UC22\] Validar a Elegibilidade do Aluno**

**Pré-condição:** 

1. O aluno candidatou-se para uma atividade acadêmica (TCC, Estágio ou Monitoria).

**Fluxo Básico:**

1. O ator acessa a solicitação de elegibilidade do aluno  
2. O sistema exibe o formulário de candidatura do aluno  
3. O ator seleciona a opção "Elegível" ou "Inelegível"  
4. O sistema solicita confirmação  
5. O ator confirma \[FA001\]  
6. O sistema registra a decisão e notifica os envolvidos na atividade correspondente

**Fluxo Alternativo:**

**1\. Cancelar operação:**  
Ocorre quando o ator não confirma a opção selecionada. A mensagem de confirmação some. Retorna ao passo 2\.

# **\[UC23\] – Visualizar lista de atividades**

**Pontos de Extensão:** 

- Filtrar atividades por ator.


**Fluxo Básico:**

1. O ator solicita a exibição da lista de atividades que participa ou orienta.  
2. Inclui o caso de uso “Verificar permissões de acesso”  
3. Ponto de extensão: Filtrar atividades por ator

**\[UC023- EXT1\] \- Acesso do professor:**

**Estende:** UC023 \- Visualizar lista de atividades.  
**Ponto de Extensão:** Filtrar atividades por ator.  
**Condição:** Ator \= Professor.

**Fluxo de extensão:**

1. O sistema coleta os metadados das atividades das quais o ator é orientador.  
2. O sistema exibe a lista das atividades coletadas \[FA01\].

**Fluxos alternativos:**

**1\. Nenhuma atividade orientada:**  
	Ocorre quando não houverem atividades nas quais o ator é orientador. O sistema exibe uma mensagem informando que não há atividades. O caso de uso é encerrado.

**\[UC023 \- EXT2\] \- Acesso do Orientando:**

**Fluxo de extensão:**

1. O sistema coleta os metadados das atividades que o ator participa.  
2. O sistema exibe a lista das atividades coletadas \[FA01\].

**Fluxos alternativos:**

**1\. Nenhuma atividade participada:**  
	Ocorre quando não houverem atividades nas quais o ator participa. O sistema exibe uma mensagem informando que não há atividades. O caso de uso é encerrado.

**\[UC023 \- EXT3\] \- Acesso do Coordenador de curso:**

**Estende:** UC023  \- Visualizar lista de atividades.  
**Ponto de Extensão:** Filtrar atividades por ator.  
**Condição:** Ator \= Coordenador de curso.

**Fluxo de extensão:**

1. O sistema coleta os metadados de todas as atividades ativas ou finalizadas do curso coordenado pelo ator.  
2. O sistema exibe a lista de todas as atividades \[FA01\].

**Fluxos alternativos:**

**1\. Nenhuma atividade ativa ou finalizada:**  
	Ocorre quando não houverem atividades ativas ou finalizadas. O sistema exibe uma mensagem informando que não há atividades. O caso de uso é encerrado.

# **\[UC24\] – Visualizar atividade**

**Pré-condição**: 

1. O ator acessou a lista de atividades por meio do caso de uso \[UC023\] \- Visualizar lista de atividades ou por meio do caso de uso \[UC016\] \- Visualizar histórico.  
   

**Fluxo Principal:**

1. O sistema exibe a lista de atividades que o ator participa ou orienta.  
2. O ator clica sobre uma atividade específica.  
3. O sistema exibe as informações da atividade específica escolhida.

# **\[UC25\] – Verificar permissões de acesso**

**Pré-condição:** 

1. O ator deve estar autenticado no sistema.  
   

**Fluxo Básico:**

1. O sistema recebe uma solicitação de acesso a um recurso  
2. O sistema identifica o ator que está fazendo a solicitação.  
3. O sistema consulta o perfil do ator no banco de dados.  
4. O sistema concede o acesso ao recurso específico do seu perfil.

# **\[UC26\] \- Visualizar lista de candidaturas**

**Pontos de Extensão:** 

- Filtrar candidaturas por ator.

**Fluxo Básico:**

1. O ator solicita a exibição da lista de candidaturas enviadas ou recebidas.  
2. Inclui o caso de uso “Verificar permissões de acesso”.  
3. Ponto de extensão: Filtrar candidaturas por ator.

**\[UC026 \- EXT1\] \- Acesso do professor:**

**Estende:** UC026 \- Visualizar lista de candidaturas.  
**Ponto de Extensão:** Filtrar candidaturas por ator.  
**Condição:** Ator \= Professor.

**Fluxo de extensão:**

1. O sistema coleta os metadados das candidaturas enviadas para o ator.  
2. O sistema exibe a lista de candidaturas coletadas \[FA01\].

**Fluxos alternativos:**

**1\. Sem solicitações enviadas:**  
Ocorre caso o ator não tenha recebido nenhuma candidatura, o sistema exibe a mensagem “Nenhuma candidatura enviada até o momento.”

**\[UC026 \- EXT2\] \- Acesso do Aluno:**

**Estende:** UC026 \- Visualizar lista de candidaturas.  
**Ponto de Extensão:** Filtrar candidaturas por ator.  
**Condição:** Ator \= Aluno.

**Fluxo de extensão:**

1. O sistema coleta os metadados das candidaturas enviadas pelo ator.  
2. O sistema exibe a lista das candidaturas coletadas \[FA01\].

**Fluxos alternativos:**

**1\. Sem solicitações enviadas:**  
Ocorre caso o ator não tenha enviado nenhuma candidatura, o sistema exibe a mensagem “Nenhuma candidatura enviada até o momento.”

# **\[UC27\] \- Visualizar candidatura**

**Pré-condição:** 

1. O ator acessou a lista de candidaturas por meio do caso de uso \[UC026\] \- Visualizar lista de candidaturas.  
   

**Fluxo Principal:**

1. O sistema exibe a lista de candidaturas enviada.  
2. O ator clica sobre uma candidatura específica.  
3. O sistema exibe as informações da candidatura específica escolhida.

# **\[UC28\] \- Validar candidaturas de atividades**

**Pré-condição:** 

1. O ator acessou uma candidatura específica de um aluno por meio do caso de uso \[UC027\] \- Visualizar candidatura.  
   

**Fluxo Principal:**

1. O sistema exibe opções de “Aprovar” ou “Rejeitar”.  
2. O ator seleciona a opção desejada. \[FE01\]  
3. O sistema pede confirmação da opção escolhida.  
4. O ator confirma a opção escolhida.   
5. O sistema registra a decisão.  
   

**Fluxo Alternativo:**

**1\. Cancelar operação:**  
Ocorre quando o ator não confirma a opção selecionada. A mensagem de confirmação some. Retorna ao passo 1\.

# **\[UC29\] \- Visualizar status do processo das candidaturas**

**Pré-condição:** 

1. O ator já deve ter se candidatado à uma atividade.  
2. O ator acessou uma candidatura específica de um aluno por meio do caso de uso \[UC027\] \- Visualizar candidatura.  
   

**Fluxo Principal:**

1. O sistema exibe a candidatura enviada.  
2. O ator seleciona a opção de visualizar o processo.   
3. O sistema exibe o status do processo da candidatura.  
   

# **\[UC30\] \- Cancelar atividade**

**Pré-condição:** 

1. O ator deve orientar à atividade.  
2. O ator acessou uma atividade específica de um aluno por meio do caso de uso \[UC024\] \- Visualizar atividade.  
   

**Fluxo Principal:**

1. O sistema exibe a atividade orientada.  
2. O ator seleciona a opção de cancelar a candidatura.  
3. O sistema pede confirmação do cancelamento. \[FA01\]  
4. O ator confirma o cancelamento.   
5. O sistema registra a decisão.  
   

**Fluxo Alternativo:**

**1\. Cancelar operação:**  
Ocorre quando o ator não confirma o cancelamento. A mensagem de confirmação some. Retorna ao passo 1\.

# **\[UC31\] \- Visualizar perfil do usuário**

**Fluxo Principal:**

1. O ator seleciona o avatar do seu perfil ou a opção perfil do usuário.  
2. O sistema exibe o perfil do usuário.

