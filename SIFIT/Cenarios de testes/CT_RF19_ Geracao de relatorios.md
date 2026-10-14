## Cenário 19: Geração de relatórios.

### Caso de Teste 01: Gerar relatório de Clientes.

| ID       | Descrição |
| :------- | :-------- |
| C19-CT01 | O sistema deve gerar o relatório de clientes. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                       |
| :--------------------------------------------------------------- |
| **DADO** que acessamos "Financeiro > Relatórios"                 |
| **E** selecionamos o tipo "Clientes"                             |
| **QUANDO** clicarmos em "Gerar Relatório"                        |
| **ENTÃO** o relatório deve ser exibido com a lista de clientes   |

| **Critérios de aceitação**              |
| :-------------------------------------- |
| O relatório deve ser gerado sem erro.   |

---

### Caso de Teste 02: Gerar relatório de Contas a Receber por período.

| ID       | Descrição |
| :------- | :-------- |
| C19-CT02 | O relatório deve respeitar as datas informadas. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                               |
| :----------------------------------------------------------------------- |
| **DADO** que estamos na tela de Relatórios                               |
| **E** selecionamos "Contas a Receber" e o primeiro e último dia do mês   |
| **QUANDO** clicarmos em "Gerar Relatório"                                |
| **ENTÃO** o relatório deve conter apenas contas do período               |

| **Critérios de aceitação**                         |
| :------------------------------------------------- |
| Nenhum lançamento fora do período deve aparecer.   |

---

### Caso de Teste 03: Relatório com data final anterior à inicial.

| ID       | Descrição |
| :------- | :-------- |
| C19-CT03 | O sistema deve validar o intervalo de datas. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                             |
| :--------------------------------------------------------------------- |
| **DADO** que estamos na tela de Relatórios                             |
| **E** informamos data inicial "31/10/2026" e data final "01/10/2026"   |
| **QUANDO** clicarmos em "Gerar Relatório"                              |
| **ENTÃO** o sistema deve exibir mensagem de período inválido           |

| **Critérios de aceitação**                              |
| :------------------------------------------------------ |
| O relatório não deve ser gerado com datas invertidas.   |
