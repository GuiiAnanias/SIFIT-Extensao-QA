## **Requisitos Funcionais Detalhados para Testes Manuais**



### **RF01 - Autenticação de Usuário**

  * O sistema deve permitir que o usuário realize login com usuário e senha válidos.

  * O sistema deve exibir mensagem de erro em caso de login inválido.

---

### **RF02 - Página Inicial e Dashboard**

**Descrição**: Após o login, o sistema deve exibir a página inicial com os principais indicadores da academia.

* **Funcionalidades esperadas**:

  * Exibição de mensalidades pendentes, agenda do dia e últimas entradas.
  * Exibição de alunos em risco e aniversariantes.
  * Navegação funcional pelo menu lateral.

---

### **RF03 - Check-in e Presenças**

**Descrição**: O sistema deve controlar a entrada dos alunos na academia.

* **Funcionalidades esperadas**:

  * Check-in manual pelo código do cliente.
  * Check-in por QR Code.
  * Consulta de presenças por dia, semana e mês.

---

### **RF04 - Gestão de Clientes**

**Descrição**: O sistema deve permitir o cadastro completo dos alunos.

* **Funcionalidades esperadas**:

  * Listagem de todos os clientes cadastrados.
  * Filtros de busca por código e nome.
  * Botão "Novo Cliente" para cadastrar um aluno.
  * Opção de visualizar ou excluir um cliente.

---

### **RF05 - Matrículas**

**Descrição**: Vincular o cliente a um plano, com as condições de pagamento.

* **Funcionalidades esperadas**:

  * Cadastro de matrícula com plano, datas, forma de pagamento e valores.
  * Filtro por código, nome e data.
  * Cancelamento e exclusão de matrículas.

---

### **RF06 - Avaliações Físicas**

**Descrição**: Registrar e acompanhar as avaliações físicas dos alunos.

* **Funcionalidades esperadas**:

  * Cadastro e alteração de avaliações.
  * Visualização dos resultados.
  * Comparação entre avaliações do mesmo aluno.

---

### **RF07 - Treinamento**

**Descrição**: Montagem das fichas de treino e organização das turmas.

* **Funcionalidades esperadas**:

  * Cadastro de fichas de treino por aluno.
  * Biblioteca de exercícios por grupo muscular.
  * Cadastro de turmas com horário e dias da semana.

---

### **RF08 - Financeiro**

**Descrição**: Controle de contas, caixa e despesas da academia.

* **Funcionalidades esperadas**:

  * Lançamento de contas a receber e a pagar.
  * Filtro por período e status (pendente, pago, vencido, cancelado).
  * Cadastro de despesas fixas.

---

### **RF09 - Comercial**

**Descrição**: Gestão de leads e dos planos oferecidos.

* **Funcionalidades esperadas**:

  * Cadastro de leads e acompanhamento por estágio.
  * Cadastro de planos com valor e duração.

---

### **RF10 - Relatórios**

**Descrição**: O sistema deve permitir a geração de relatórios diversos (clientes, matrículas, financeiro etc.).

* **Funcionalidades esperadas**:

  * Escolha do tipo de relatório.
  * Filtro por data inicial e final.

---

### **RF11 - Gestão**

**Descrição**: Cadastros internos da academia.

* **Funcionalidades esperadas**:

  * Cadastro e busca de colaboradores.
  * Cadastro de produtos para venda ou pontuação.

---

### **RF12 - Anamnese**

**Descrição**: Questionário de saúde dos alunos.

* **Funcionalidades esperadas**:

  * Criação de fichas de anamnese por aluno.
  * Filtro por status (concluído ou pendente).