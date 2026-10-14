## Cenário 24: Atividades, pontuação e produtos.

### Caso de Teste 01: Cadastrar atividade com pontuação.

| ID       | Descrição |
| :------- | :-------- |
| C24-CT01 | O sistema deve cadastrar uma atividade que gera pontos. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                      |
| :------------------------------------------------------------------------------ |
| **DADO** que acessamos "Gestão > Atividades"                                    |
| **E** clicamos em "Nova Atividade"                                              |
| **E** preenchemos o nome "Atividade Teste QA", a descrição e a pontuação "10"   |
| **QUANDO** clicarmos em "Salvar"                                                |
| **ENTÃO** a atividade deve aparecer na listagem com a pontuação informada       |

| **Critérios de aceitação**      |
| :------------------------------ |
| A atividade deve ser listada.   |

---

### Caso de Teste 02: Cadastrar produto do tipo Venda.

| ID       | Descrição |
| :------- | :-------- |
| C24-CT02 | O sistema deve cadastrar um produto de venda. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                  |
| :-------------------------------------------------------------------------- |
| **DADO** que acessamos "Gestão > Produtos"                                  |
| **E** clicamos em "Novo"                                                    |
| **E** preenchemos o nome "Produto Teste QA", tipo "Venda" e valor "10,00"   |
| **QUANDO** clicarmos em "Salvar"                                            |
| **ENTÃO** o produto deve aparecer com tipo Venda e o valor informado        |

| **Critérios de aceitação**               |
| :--------------------------------------- |
| O produto deve ser listado como Ativo.   |

---

### Caso de Teste 03: Filtrar produtos por tipo.

| ID       | Descrição |
| :------- | :-------- |
| C24-CT03 | O filtro deve separar produtos de Venda e Pontuação. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                       |
| :--------------------------------------------------------------- |
| **DADO** que acessamos "Gestão > Produtos"                       |
| **E** selecionamos o tipo "Pontuação"                            |
| **QUANDO** clicarmos no botão de busca                           |
| **ENTÃO** apenas produtos do tipo Pontuação devem ser exibidos   |

| **Critérios de aceitação**           |
| :----------------------------------- |
| O resultado deve respeitar o tipo.   |
