## Cenário 15: Contas a pagar.

### Caso de Teste 01: Lançar conta a pagar.

| ID       | Descrição |
| :------- | :-------- |
| C15-CT01 | O sistema deve registrar uma conta a pagar. |

| **Pré-condições**                     |
| :------------------------------------ |
| Deve existir fornecedor cadastrado.   |

| **Passos**                                                                  |
| :-------------------------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Contas a Pagar"              |
| **E** clicamos em "Nova Conta"                                              |
| **E** preenchemos fornecedor, título "Conta Teste QA", valor e vencimento   |
| **QUANDO** clicarmos em "Salvar"                                            |
| **ENTÃO** a conta deve aparecer na listagem com status Pendente             |

| **Critérios de aceitação**               |
| :--------------------------------------- |
| A conta deve ser listada corretamente.   |

---

### Caso de Teste 02: Filtrar contas pagas.

| ID       | Descrição |
| :------- | :-------- |
| C15-CT02 | O filtro deve exibir apenas contas pagas. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                       |
| :--------------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Contas a Pagar"   |
| **E** selecionamos o status "Pago"                               |
| **QUANDO** clicarmos em "Buscar"                                 |
| **ENTÃO** apenas contas pagas devem ser exibidas                 |

| **Critérios de aceitação**             |
| :------------------------------------- |
| O resultado deve respeitar o status.   |

---

### Caso de Teste 03: Lançar conta sem fornecedor.

| ID       | Descrição |
| :------- | :-------- |
| C15-CT03 | O sistema deve bloquear conta sem fornecedor ou colaborador. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Contas a Pagar"                |
| **E** clicamos em "Nova Conta"                                                |
| **E** deixamos o fornecedor/colaborador em branco                             |
| **QUANDO** clicarmos em "Salvar"                                              |
| **ENTÃO** mensagens de validação devem ser exibidas nos campos obrigatórios   |

| **Critérios de aceitação**       |
| :------------------------------- |
| Nenhuma conta deve ser criada.   |
