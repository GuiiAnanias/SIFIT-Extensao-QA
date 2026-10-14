## Cenário 21: Planos e formas de pagamento.

### Caso de Teste 01: Cadastrar plano sem nome e valor.

| ID       | Descrição |
| :------- | :-------- |
| C21-CT01 | O sistema deve bloquear plano incompleto. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Comercial > Planos"                                   |
| **E** clicamos em "Novo Plano"                                                |
| **E** deixamos nome e valor em branco                                         |
| **QUANDO** clicarmos em "Salvar"                                              |
| **ENTÃO** mensagens de validação devem ser exibidas nos campos obrigatórios   |

| **Critérios de aceitação**      |
| :------------------------------ |
| Nenhum plano deve ser criado.   |

---

### Caso de Teste 02: Filtrar tipos de pagamento.

| ID       | Descrição |
| :------- | :-------- |
| C21-CT02 | O filtro deve separar débito e crédito. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                |
| :-------------------------------------------------------- |
| **DADO** que acessamos "Comercial > Tipos de Pagamento"   |
| **QUANDO** selecionarmos o tipo "Crédito"                 |
| **ENTÃO** apenas tipos de crédito devem ser exibidos      |

| **Critérios de aceitação**           |
| :----------------------------------- |
| O resultado deve respeitar o tipo.   |

---

### Caso de Teste 03: Cadastrar bandeira de cartão.

| ID       | Descrição |
| :------- | :-------- |
| C21-CT03 | O sistema deve cadastrar uma bandeira. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                       |
| :----------------------------------------------- |
| **DADO** que acessamos "Comercial > Bandeiras"   |
| **E** clicamos em "Nova Bandeira"                |
| **E** preenchemos o nome "Bandeira Teste QA"     |
| **QUANDO** clicarmos em "Salvar"                 |
| **ENTÃO** a bandeira deve aparecer na listagem   |

| **Critérios de aceitação**     |
| :----------------------------- |
| A bandeira deve ser listada.   |
