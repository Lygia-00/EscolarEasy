# EscolarEasy

## Descrição do Projeto

O **Escolar Easy** é uma aplicação abrangente desenvolvida para simplificar a gestão acadêmica, proporcionando uma solução fácil e eficiente para o controle de notas, matrículas e matérias de alunos. Com uma interface intuitiva e recursos poderosos, esta aplicação foi projetada para facilitar as tarefas administrativas em ambientes educacionais.

## Casos de Uso

### Realizar Cadastro

**Cenário do Caso de Uso**

- Pré-condição: O usuário acessou a página da universidade.
- Pós-condição: O usuário é cadastrado e seus dados são armazenados no sistema.

**Cenário de Sucesso Principal:**

1. O usuário acessa a página de cadastro da universidade.
2. O sistema apresenta a página de cadastro.
3. O usuário preenche todos os campos obrigatórios.
4. O usuário seleciona uma das opções disponíveis: “Pessoa Física”, “Pessoa Jurídica”, “Professor” ou “Fornecedor”.
5. O usuário clica no botão cadastrar.
6. O sistema retorna informando que o cadastro foi concluído com sucesso.
7. O sistema envia notificação ao e-mail cadastrado com as informações de acesso do usuário.

**Fluxos Alternativos:**
- (2-5): O usuário desiste do cadastro, cancelando-o.
- (4): O sistema informa que o usuário já está cadastrado.

### Acessar Perfil

**Cenário do Caso de Uso**

- Pré-condição: O usuário acessou a página da universidade; O usuário finalizou o caso “Realizar cadastro” com sucesso.
- Pós-condição: O usuário visualiza as informações cadastradas em seu perfil.

**Cenário de Sucesso Principal:**

1. O usuário acessa a página de login da universidade.
2. O sistema apresenta a página de login pedindo a identificação do usuário e senha.
3. O usuário informa sua identificação de usuário e senha.
4. O sistema apresenta a página do Perfil do usuário.

**Fluxos Alternativos:**
- (3): O usuário digitou alguma informação de identificação incorreta. O sistema informa que as credenciais estão incorretas.
- (3): O usuário informou as credenciais incorretas pela terceira vez. O sistema bloqueia o usuário e envia uma notificação ao e-mail cadastrado com informações para reestabelecer o acesso.

### Atualizar Dados

**Cenário do Caso de Uso**

- Pré-condição: O usuário acessou a página da universidade; O usuário finalizou o caso “Acessar perfil” com sucesso.
- Pós-condição: As informações do usuário são alteradas no sistema.

**Cenário de Sucesso Principal:**

1. O usuário clica no botão “Informações cadastrais”.
2. O usuário altera suas informações de cadastro.
3. O usuário clica no botão “Salvar alterações”.
4. O sistema armazena os dados alterados.
5. O sistema retorna informando que os dados foram alterados com sucesso.

**Fluxos Alternativos:**
- (3): Usuário informou um endereço de e-mail inválido. O sistema retorna informando que o formato do endereço está incorreto. Os dados não são alterados e salvos.
- (3): Usuário informou o CNPJ inválido. O sistema retorna informando que o formato está incorreto. Os dados não são alterados e salvos.

### Lançar Notas

**Cenário do Caso de Uso**

- Pré-condição: O professor está autenticado na página da universidade.
- Pós-condição: As notas dos alunos são lançadas no sistema.

**Cenário de Sucesso Principal:**

1. O professor escolhe a opção “Lançar notas”.
2. O sistema apresenta a tela de escolha de turmas.
3. O professor seleciona a turma desejada.
4. O sistema apresenta a lista de avaliações disponíveis para a turma.
5. O professor escolhe a avaliação para a qual deseja lançar as notas.
6. O sistema apresenta a página com a lista de alunos da turma que fizeram a avaliação.
7. O professor preenche as notas dos alunos da lista.
8. O professor clica no botão “Atualizar notas”.
9. O sistema grava os dados informados.
10. O sistema retorna informando que as notas foram lançadas com sucesso.

**Fluxos Alternativos:**
- (8): O professor inseriu notas diferentes do formato especificado e esperado. O sistema retorna informando que o formato das notas está no formato incorreto. Os dados não são atualizados.
- (8): O professor ficou muito tempo sem informar nenhuma nota. O sistema cancelou a sessão do usuário. Os dados não são gravados. O sistema retorna para a tela de autenticação.

### Visualizar Histórico Acadêmico

**Cenário do Caso de Uso**

- Pré-condição: O usuário acessou a página da universidade.
- Pós-condição: O usuário visualiza seu histórico acadêmico.

**Cenário de Sucesso Principal:**

1. O usuário acessa a página de histórico acadêmico da universidade.
2. O sistema apresenta a página com as opções de consulta ao histórico.
3. O usuário fornece as informações necessárias, como número de matrícula, ano letivo, ou outro identificador válido.
4. O sistema recupera e exibe o histórico acadêmico do usuário, incluindo informações como cursos realizados, notas, créditos e qualquer outra informação relevante.
5. Os usuários podem optar por imprimir ou baixar transcrições.

**Fluxos Alternativos:**
- (3): Se as informações fornecidas pelo usuário não forem válidas, o sistema informa sobre o erro.
- (4): Se não houver histórico acadêmico disponível para as informações fornecidas, o sistema informa que não há dados para exibir.

### Atualizar Informações Acadêmicas

**Cenário do Caso de Uso**

- Pré-condição: O usuário acessou a página da universidade e está autenticado em sua conta.
- Pós-condição: As informações acadêmicas do usuário são atualizadas no sistema.

**Cenário de Sucesso Principal:**

1. O usuário acessa a página de atualização de informações acadêmicas.
2. O sistema exibe um formulário preenchido com as informações acadêmicas atuais do usuário.
3. O usuário modifica as informações desejadas, como mudança de curso, adição de disciplinas, ou alteração de dados pessoais relacionados à sua vida acadêmica.
4. O usuário confirma as alterações.
5. O sistema valida as informações e atualiza o registro acadêmico do usuário.
6. O sistema retorna uma confirmação de que as informações foram atualizadas com sucesso.

**Fluxos Alternativos:**
- (3): Se o sistema detectar informações inválidas, o usuário é informado sobre o erro e orientado sobre como corrigir.
- (5): Caso ocorra algum erro durante o processo de atualização, o sistema informa o usuário sobre a falha e fornece orientações sobre como proceder.
