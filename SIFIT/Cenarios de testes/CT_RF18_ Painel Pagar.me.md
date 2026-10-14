## Cenário 18: Painel Pagar.me.

### Caso de Teste 01: Visualizar painel de recebimentos.

| ID       | Descrição |
| :------- | :-------- |
| C18-CT01 | A tela deve exibir o resumo dos recebimentos. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                                                                |
| :------------------------------------------------------------------------------------------------------------------------ |
| **DADO** que acessamos "Financeiro > Pagar.me"                                                                            |
| **QUANDO** a tela for carregada                                                                                           |
| **ENTÃO** devem ser exibidos Recebimentos, Meios de pagamento, Transações recentes, Repasses, Assinaturas e Chargebacks   |

| **Critérios de aceitação**                 |
| :----------------------------------------- |
| Todos os blocos devem carregar sem erro.   |

---

### Caso de Teste 02: Filtrar recebimentos por período.

| ID       | Descrição |
| :------- | :-------- |
| C18-CT02 | O painel deve atualizar os valores pelo período. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                            |
| :-------------------------------------------------------------------- |
| **DADO** que acessamos "Financeiro > Pagar.me"                        |
| **QUANDO** selecionarmos "Últimos 30 dias"                            |
| **ENTÃO** os valores devem ser atualizados para o período escolhido   |

| **Critérios de aceitação**                  |
| :------------------------------------------ |
| Os valores devem corresponder ao período.   |

---

### Caso de Teste 03: Consultar todas as transações.

| ID       | Descrição |
| :------- | :-------- |
| C18-CT03 | O sistema deve listar o histórico de transações. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                       |
| :------------------------------------------------------------------------------- |
| **DADO** que acessamos "Financeiro > Pagar.me"                                   |
| **QUANDO** clicarmos em "Ver todas as transações"                                |
| **ENTÃO** a lista deve exibir Data, Descrição, Cliente, Valor, Método e Status   |

| **Critérios de aceitação**        |
| :-------------------------------- |
| A listagem deve abrir sem erro.   |
