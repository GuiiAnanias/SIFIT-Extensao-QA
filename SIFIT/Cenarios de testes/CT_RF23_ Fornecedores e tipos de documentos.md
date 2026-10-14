## Cenário 23: Fornecedores e tipos de documentos.

### Caso de Teste 01: Cadastrar fornecedor.

| ID       | Descrição |
| :------- | :-------- |
| C23-CT01 | O sistema deve cadastrar um fornecedor. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                         |
| :------------------------------------------------- |
| **DADO** que acessamos "Gestão > Fornecedores"     |
| **E** clicamos em "Novo Fornecedor"                |
| **E** preenchemos o nome "Fornecedor Teste QA"     |
| **QUANDO** clicarmos em "Salvar"                   |
| **ENTÃO** o fornecedor deve aparecer na listagem   |

| **Critérios de aceitação**       |
| :------------------------------- |
| O fornecedor deve ser listado.   |

---

### Caso de Teste 02: Cadastrar fornecedor sem nome.

| ID       | Descrição |
| :------- | :-------- |
| C23-CT02 | O sistema deve bloquear fornecedor sem nome. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Gestão > Fornecedores"                                |
| **E** clicamos em "Novo Fornecedor"                                           |
| **E** deixamos o nome em branco                                               |
| **QUANDO** clicarmos em "Salvar"                                              |
| **ENTÃO** mensagens de validação devem ser exibidas nos campos obrigatórios   |

| **Critérios de aceitação**           |
| :----------------------------------- |
| Nenhum fornecedor deve ser criado.   |

---

### Caso de Teste 03: Filtrar tipos de documento por aplicação.

| ID       | Descrição |
| :------- | :-------- |
| C23-CT03 | O filtro deve separar documentos de conta e de colaborador. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                              |
| :---------------------------------------------------------------------- |
| **DADO** que acessamos "Gestão > Tipos de Documentos"                   |
| **QUANDO** selecionarmos a aplicação "Colaborador"                      |
| **ENTÃO** apenas tipos de documento de colaborador devem ser exibidos   |

| **Critérios de aceitação**                |
| :---------------------------------------- |
| O resultado deve respeitar a aplicação.   |
