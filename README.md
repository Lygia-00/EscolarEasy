# EscolarEasy
## Descrição do Projeto
O Escolar Easy é uma aplicação abrangente desenvolvida para simplificar a gestão acadêmica, fornecendo uma solução fácil e eficiente para o controle de notas, matrículas e matérias de alunos. Com uma interface intuitiva e recursos poderosos, esta aplicação foi projetada para facilitar as tarefas administrativas em ambientes educacionais.

## Funcionalidades Principais

### Realizar Cadastro

**Descrição:**
- Permita que novos usuários, sejam eles alunos, professores, ou colaboradores, realizem o cadastro na plataforma.

**Cenário de Sucesso Principal:**
1. O usuário acessa a página de cadastro.
2. O sistema apresenta os campos necessários para preenchimento.
3. O usuário preenche todas as informações obrigatórias.
   - **Campo Específico:** Para o campo "Documento" (CPF ou CNPJ), foi implementada uma máscara para facilitar o preenchimento.
4. Seleciona o tipo de cadastro: "Aluno", "Professor" ou "Colaborador".
5. Clica no botão de cadastro.
6. O sistema confirma o cadastro e envia uma notificação ao e-mail cadastrado.

**Fluxos Alternativos:**
- (2-5) A qualquer momento, o usuário pode desistir do cadastro, cancelando-o e não salvando os dados.
- (4) O sistema informa se o usuário já está cadastrado.

### Acessar Perfil

**Descrição:**
- Fornece aos usuários a capacidade de acessar seu perfil após o cadastro.

**Cenário de Sucesso Principal:**
1. O usuário acessa a página de login.
2. Informa identificação de usuário e senha.
3. O sistema valida as credenciais e apresenta o perfil do usuário.

**Fluxos Alternativos:**
- (3) Se as credenciais estiverem incorretas, o sistema notifica o usuário.
- (3) Após três tentativas incorretas, o sistema bloqueia o usuário e envia informações de reestabelecimento de acesso ao e-mail cadastrado.

### Receber Pagamentos

**Descrição:**
- Possibilita à instituição receber pagamentos relacionados a taxas e mensalidades.

### Enviar Orçamento

**Descrição:**
- Permite o envio de orçamentos, facilitando a comunicação transparente entre a instituição e os envolvidos.

### Lançar Notas

**Descrição:**
- Capacita os professores a lançarem notas e avaliações para os alunos, proporcionando um acompanhamento preciso do desempenho acadêmico.

### Atualizar Dados

**Descrição:**
- Oferece a funcionalidade de atualizar dados pessoais dos usuários, mantendo informações precisas no sistema.

### Realizar Cadastros e Matrículas

**Descrição:**
- Permite a realização de cadastros adicionais e matrículas em cursos, disciplinas e eventos acadêmicos.

### Atualizar Informações

**Descrição:**
- Permite a atualização de diversas informações, desde dados pessoais até preferências de contato e notificações.

### Acessar Histórico Acadêmico

**Descrição:**
- Fornece aos usuários acesso ao seu histórico acadêmico, contendo informações sobre cursos, disciplinas cursadas e notas obtidas.

### Atualizar Informações Institucionais

**Descrição:**
- Reservada para administradores, esta funcionalidade permite a atualização de informações institucionais relevantes para a comunidade acadêmica.
