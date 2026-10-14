## Cenário 17: Despesas fixas.

### Caso de Teste 01: Cadastrar despesa fixa.

| ID       | Descrição |
| :------- | :-------- |
| C17-CT01 | O sistema deve cadastrar uma despesa recorrente. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                         |
| :--------------------------------------------------------------------------------- |
| **DADO** que acessamos "Financeiro > Despesas Fixas"                               |
| **E** clicamos em "Nova Despesa"                                                   |
| **E** preenchemos o nome "Despesa Teste QA", valor "50,00" e recorrência "1 Mês"   |
| **QUANDO** clicarmos em "Salvar"                                                   |
| **ENTÃO** a despesa deve aparecer na listagem com status Ativo                     |

| **Critérios de aceitação**                            |
| :---------------------------------------------------- |
| A despesa deve ser listada com valor e recorrência.   |

---

### Caso de Teste 02: Despesa com valor negativo.

| ID       | Descrição |
| :------- | :-------- |
| C17-CT02 | O sistema não deve aceitar valor negativo. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                   |
| :----------------------------------------------------------- |
| **DADO** que acessamos "Financeiro > Despesas Fixas"         |
| **E** clicamos em "Nova Despesa"                             |
| **E** preenchemos o nome e o valor "-50,00"                  |
| **QUANDO** clicarmos em "Salvar"                             |
| **ENTÃO** o sistema deve exibir mensagem de valor inválido   |

| **Critérios de aceitação**                 |
| :----------------------------------------- |
| Nenhuma despesa negativa deve ser salva.   |

---

### Caso de Teste 03: Filtrar despesas por recorrência.

| ID       | Descrição |
| :------- | :-------- |
| C17-CT03 | O filtro deve exibir apenas a recorrência escolhida. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                             |
| :----------------------------------------------------- |
| **DADO** que acessamos "Financeiro > Despesas Fixas"   |
| **E** selecionamos a recorrência "1 Mês"               |
| **QUANDO** clicarmos em "Buscar"                       |
| **ENTÃO** apenas despesas mensais devem ser exibidas   |

| **Critérios de aceitação**                  |
| :------------------------------------------ |
| O resultado deve respeitar a recorrência.   |
