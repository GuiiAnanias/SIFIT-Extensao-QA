## **Requisitos Funcionais Detalhados para Testes Manuais**



### **RF01 - Autenticação de Usuário**

  * O sistema deve permitir que o usuário realize login com usuário e senha válidos.

  * O sistema deve exibir mensagem de erro em caso de login inválido.

---

### **RF02 - Página Inicial e Dashboard**

**Descrição**: Após o login, o sistema deve exibir a página inicial com os principais indicadores da academia.

* **Funcionalidades esperadas**:

  * Exibição de mensalidades pendentes, agenda do dia, últimas entradas e aniversariantes.
  * Dashboard com alunos em risco, avaliações vencendo e frequência em queda.
  * Navegação funcional pelo menu lateral.

---

### **RF03 - Check-in**

**Descrição**: O sistema deve controlar a entrada dos alunos na academia.

* **Funcionalidades esperadas**:

  * Check-in manual pelo código do cliente.
  * Check-in por QR Code.
  * Filtros: presentes agora, não compareceram e check-in pendente.

---

### **RF04 - Presenças**

**Descrição**: Consulta do histórico de entradas dos alunos.

* **Funcionalidades esperadas**:

  * Busca por cliente.
  * Filtros por hoje, semana e mês.

---

### **RF05 - Clientes**

**Descrição**: O sistema deve permitir o cadastro completo dos alunos.

* **Funcionalidades esperadas**:

  * Listagem de todos os clientes cadastrados.
  * Filtros de busca por código e nome.
  * Botão "Novo Cliente" com os campos obrigatórios nome, status, sexo e data de nascimento.
  * Opção de visualizar ou excluir um cliente.

---

### **RF06 - Matrículas**

**Descrição**: Vincular o cliente a um plano, com as condições de pagamento.

* **Funcionalidades esperadas**:

  * Cadastro de matrícula com modalidade, datas, forma de pagamento e valores.
  * Filtro por código, nome e data.
  * Cancelamento e exclusão de matrículas.

---

### **RF07 - Avaliações Físicas**

**Descrição**: Registrar e acompanhar as avaliações físicas dos alunos.

* **Funcionalidades esperadas**:

  * Cadastro e alteração de avaliações.
  * Visualização e envio por link.
  * Comparação entre avaliações do mesmo aluno.

---

### **RF08 - Fichas de Treino e Modelos de Ficha**

**Descrição**: Montagem dos treinos dos alunos.

* **Funcionalidades esperadas**:

  * Cadastro de ficha por aluno com data inicial e final.
  * Filtro por status (ativo, inativo, cancelado, finalizado).
  * Consulta dos modelos de ficha.

---

### **RF09 - Exercícios**

**Descrição**: Biblioteca de exercícios usada nas fichas.

* **Funcionalidades esperadas**:

  * Cadastro de exercício por grupo muscular.
  * Visualização e exclusão de exercícios.

---

### **RF10 - Grupos Musculares e Objetivos de Treino**

**Descrição**: Cadastros de apoio do treinamento.

* **Funcionalidades esperadas**:

  * Cadastro de grupo muscular com tipo de membro (inferiores, superiores, aeróbio).
  * Filtro por tipo de membro.
  * Cadastro de objetivos de treino.

---

### **RF11 - Turmas e Grupos**

**Descrição**: Organização das turmas e dos grupos da academia.

* **Funcionalidades esperadas**:

  * Cadastro de turma com plano, horário e dias da semana.
  * Edição e exclusão de turmas.
  * Cadastro de grupos com tipo interno ou externo.

---

### **RF12 - SifitBox**

**Descrição**: Gestão das aulas do box (crossfit).

* **Funcionalidades esperadas**:

  * Geração das aulas por data.
  * Cadastro de modalidades.
  * Cadastro de turmas recorrentes com horário, dias e vagas.

---

### **RF13 - Categorias Crossfit**

**Descrição**: Categorias dos exercícios de crossfit.

* **Funcionalidades esperadas**:

  * Cadastro, edição e exclusão de categorias.
  * Busca por código e nome.

---

### **RF14 - Contas a Receber**

**Descrição**: Controle dos valores a receber dos clientes.

* **Funcionalidades esperadas**:

  * Lançamento de nova conta.
  * Filtro por período e status (pendente, recebido, vencido, cancelado).

---

### **RF15 - Contas a Pagar**

**Descrição**: Controle das despesas com fornecedores e colaboradores.

* **Funcionalidades esperadas**:

  * Lançamento de nova conta.
  * Filtro por período e status (pendente, pago, vencido, cancelado).

---

### **RF16 - Caixas**

**Descrição**: Controle do movimento de caixa.

* **Funcionalidades esperadas**:

  * Abertura de caixa.
  * Visualização e impressão do caixa.
  * Filtro por status (aberto, fechado).

---

### **RF17 - Despesas Fixas**

**Descrição**: Cadastro das despesas recorrentes da academia.

* **Funcionalidades esperadas**:

  * Cadastro de despesa com valor e recorrência.
  * Filtro por status e recorrência.

---

### **RF18 - Pagar.me**

**Descrição**: Painel da integração de pagamentos.

* **Funcionalidades esperadas**:

  * Resumo de recebimentos, repasses, assinaturas e chargebacks.
  * Filtro por período.
  * Lista de transações recentes.

---

### **RF19 - Relatórios**

**Descrição**: O sistema deve permitir a geração de relatórios diversos (avaliações, clientes, colaboradores, matrículas, contas e caixas).

* **Funcionalidades esperadas**:

  * Escolha do tipo de relatório.
  * Filtro por data inicial e final.

---

### **RF20 - Prospecção**

**Descrição**: Controle dos leads (possíveis alunos).

* **Funcionalidades esperadas**:

  * Cadastro de leads.
  * Acompanhamento por estágio (novo contato, interessado, aula experimental, proposta, fechado).
  * Busca por nome, e-mail, telefone ou código.

---

### **RF21 - Planos e Formas de Pagamento**

**Descrição**: Planos oferecidos e configurações de pagamento.

* **Funcionalidades esperadas**:

  * Cadastro de planos com valor e duração.
  * Modelos de contrato.
  * Tipos de pagamento (débito ou crédito) e bandeiras de cartão.

---

### **RF22 - Colaboradores e Funções**

**Descrição**: Cadastro da equipe da academia.

* **Funcionalidades esperadas**:

  * Cadastro e busca de colaboradores.
  * Cadastro de funções com permissões.

---

### **RF23 - Fornecedores e Tipos de Documentos**

**Descrição**: Cadastros usados no financeiro.

* **Funcionalidades esperadas**:

  * Cadastro e busca de fornecedores.
  * Tipos de documento para conta/fornecedor ou colaborador.

---

### **RF24 - Atividades, Pontuação e Produtos**

**Descrição**: Programa de pontos e produtos da academia.

* **Funcionalidades esperadas**:

  * Cadastro de atividades que geram pontuação.
  * Cadastro de pontuações.
  * Cadastro de produtos para venda ou troca por pontos.

---

### **RF25 - Enquetes**

**Descrição**: Pesquisas enviadas aos alunos.

* **Funcionalidades esperadas**:

  * Cadastro de enquete com pergunta.
  * Filtro por status.

---

### **RF26 - Anamnese**

**Descrição**: Questionário de saúde dos alunos.

* **Funcionalidades esperadas**:

  * Criação de fichas de anamnese por aluno.
  * Cadastro de modelos, categorias e perguntas.
  * Filtro por status (concluído ou pendente).

---

### **RF27 - Inteligência e Automação**

**Descrição**: Automações e análises feitas pelo sistema.

* **Funcionalidades esperadas**:

  * Central com automações ativas e disponíveis.
  * Resultados por período.

---

### **RF28 - Aplicativo**

**Descrição**: Gestão do aplicativo dos alunos.

* **Funcionalidades esperadas**:

  * Consulta de notificações.
  * Moderação de postagens e denúncias.

---

### **RF29 - Configurações**

**Descrição**: Configurações gerais do sistema.

* **Funcionalidades esperadas**:

  * Abas Home, Biometria, Avaliação, Aniversário, Pagamento, Integrações e Design.
  * Salvar ou cancelar alterações.
