## Cenário 06: Cadastro de matrículas.

### Caso de Teste 01: Cadastrar matrícula para cliente.

| ID       | Descrição |
| :------- | :-------- |
| C06-CT01 | O sistema deve vincular o cliente a uma modalidade. |

| **Pré-condições**                                     |
| :---------------------------------------------------- |
| O cliente "Cliente Teste QA" deve estar cadastrado.   |

| **Passos**                                                                                |
| :---------------------------------------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Matrículas"                                |
| **E** clicamos em "Cadastrar Matrícula"                                                   |
| **E** buscamos o cliente de teste pela lupa                                               |
| **E** preenchemos Modalidade, Data Inicial, Data Final, Tipo Pagamento e Dia Vencimento   |
| **QUANDO** clicarmos em "Salvar"                                                          |
| **ENTÃO** a matrícula deve aparecer na listagem vinculada ao cliente                      |

| **Critérios de aceitação**                             |
| :----------------------------------------------------- |
| A matrícula deve ser salva com Valor Total coerente.   |

---

### Caso de Teste 02: Salvar matrícula sem cliente.

| ID       | Descrição |
| :------- | :-------- |
| C06-CT02 | O sistema deve impedir matrícula sem cliente. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Matrículas"                    |
| **E** clicamos em "Cadastrar Matrícula"                                       |
| **E** deixamos o cliente em branco                                            |
| **QUANDO** clicarmos em "Salvar"                                              |
| **ENTÃO** mensagens de validação devem ser exibidas nos campos obrigatórios   |

| **Critérios de aceitação**                       |
| :----------------------------------------------- |
| Nenhuma matrícula deve ser criada sem cliente.   |

---

### Caso de Teste 03: Desconto maior que o valor.

| ID       | Descrição |
| :------- | :-------- |
| C06-CT03 | O valor total não pode ficar negativo. |

| **Pré-condições**                                     |
| :---------------------------------------------------- |
| O cliente "Cliente Teste QA" deve estar cadastrado.   |

| **Passos**                                                               |
| :----------------------------------------------------------------------- |
| **DADO** que estamos preenchendo uma matrícula para o cliente de teste   |
| **E** informamos Valor Parcela "100,00" e Desconto "150,00"              |
| **QUANDO** clicarmos em "Salvar"                                         |
| **ENTÃO** o sistema deve bloquear o salvamento ou limitar o desconto     |

| **Critérios de aceitação**                 |
| :----------------------------------------- |
| O Valor Total nunca deve ficar negativo.   |
