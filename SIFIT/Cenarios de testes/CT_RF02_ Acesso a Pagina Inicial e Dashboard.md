## Cenário 02: Acesso à Página Inicial e Dashboard.

### Caso de Teste 01: Exibição dos widgets da Página Inicial.

| ID       | Descrição |
| :------- | :-------- |
| C02-CT01 | A Página Inicial deve exibir os widgets após o login. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                                                                    |
| :---------------------------------------------------------------------------------------------------------------------------- |
| **DADO** que realizamos o login com sucesso                                                                                   |
| **QUANDO** a Página Inicial for carregada                                                                                     |
| **ENTÃO** devem ser exibidos: Mensalidades pendentes, Agenda de hoje, Últimas entradas na academia e Aniversariantes do dia   |

| **Critérios de aceitação**                  |
| :------------------------------------------ |
| Todos os widgets devem carregar sem erro.   |

---

### Caso de Teste 02: Acesso ao Dashboard pelo menu.

| ID       | Descrição |
| :------- | :-------- |
| C02-CT02 | O item Dashboard deve abrir a tela de indicadores com o título correto. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                                                                                       |
| :----------------------------------------------------------------------------------------------------------------------------------------------- |
| **DADO** que estamos na Página Inicial                                                                                                           |
| **QUANDO** clicarmos em "Principal > Dashboard"                                                                                                  |
| **ENTÃO** a tela deve exibir o título "Dashboard" e os indicadores Alunos em risco, Aniversariantes, Avaliações vencendo e Frequência em queda   |

| **Critérios de aceitação**                                      |
| :-------------------------------------------------------------- |
| O título da página deve corresponder ao item de menu clicado.   |

---

### Caso de Teste 03: Navegação pelo menu lateral.

| ID       | Descrição |
| :------- | :-------- |
| C02-CT03 | Cada item do menu deve abrir a tela correspondente. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                              |
| :---------------------------------------------------------------------- |
| **DADO** que estamos na Página Inicial                                  |
| **QUANDO** clicarmos em cada item do menu lateral                       |
| **ENTÃO** cada tela deve abrir sem erro e com o título correspondente   |

| **Critérios de aceitação**                              |
| :------------------------------------------------------ |
| A navegação deve funcionar em todos os itens do menu.   |
