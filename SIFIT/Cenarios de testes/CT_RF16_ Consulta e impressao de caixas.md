## Cenário 16: Consulta e impressão de caixas.

### Caso de Teste 01: Filtrar caixas por status.

| ID       | Descrição |
| :------- | :-------- |
| C16-CT01 | O filtro deve separar caixas abertos e fechados. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                            |
| :---------------------------------------------------- |
| **DADO** que acessamos "Financeiro > Caixas"          |
| **E** selecionamos o status "Fechado"                 |
| **QUANDO** clicarmos em "Buscar"                      |
| **ENTÃO** apenas caixas fechados devem ser exibidos   |

| **Critérios de aceitação**             |
| :------------------------------------- |
| O resultado deve respeitar o status.   |

---

### Caso de Teste 02: Visualizar caixa.

| ID       | Descrição |
| :------- | :-------- |
| C16-CT02 | O sistema deve exibir o movimento de um caixa. |

| **Pré-condições**             |
| :---------------------------- |
| Deve existir caixa fechado.   |

| **Passos**                                                            |
| :-------------------------------------------------------------------- |
| **DADO** que acessamos "Financeiro > Caixas"                          |
| **QUANDO** clicarmos em "Visualizar" em um caixa                      |
| **ENTÃO** as entradas, saídas e o saldo do caixa devem ser exibidos   |

| **Critérios de aceitação**                 |
| :----------------------------------------- |
| O saldo deve bater com as movimentações.   |

---

### Caso de Teste 03: Imprimir caixa.

| ID       | Descrição |
| :------- | :-------- |
| C16-CT03 | O sistema deve gerar a impressão do caixa. |

| **Pré-condições**             |
| :---------------------------- |
| Deve existir caixa fechado.   |

| **Passos**                                                       |
| :--------------------------------------------------------------- |
| **DADO** que acessamos "Financeiro > Caixas"                     |
| **QUANDO** clicarmos em "Imprimir" em um caixa                   |
| **ENTÃO** a tela de impressão deve abrir com os dados do caixa   |

| **Critérios de aceitação**                                 |
| :--------------------------------------------------------- |
| A impressão deve conter os mesmos dados da visualização.   |
