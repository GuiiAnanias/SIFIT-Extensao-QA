## Cenário 14: Contas a receber.

### Caso de Teste 01: Lançar conta a receber.

| ID       | Descrição |
| :------- | :-------- |
| C14-CT01 | O sistema deve registrar uma conta a receber. |

| **Pré-condições**                                     |
| :---------------------------------------------------- |
| O cliente "Cliente Teste QA" deve estar cadastrado.   |

| **Passos**                                                                     |
| :----------------------------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Contas a Receber"               |
| **E** clicamos em "Nova Conta"                                                 |
| **E** preenchemos cliente, título "Mensalidade Teste QA", valor e vencimento   |
| **QUANDO** clicarmos em "Salvar"                                               |
| **ENTÃO** a conta deve aparecer na listagem com status Pendente                |

| **Critérios de aceitação**                                    |
| :------------------------------------------------------------ |
| A conta deve ser listada com valor e vencimento informados.   |

---

### Caso de Teste 02: Filtrar contas por status e período.

| ID       | Descrição |
| :------- | :-------- |
| C14-CT02 | Os filtros devem retornar apenas as contas do status e período. |

| **Pré-condições**                |
| :------------------------------- |
| Deve existir a conta de teste.   |

| **Passos**                                                         |
| :----------------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Contas a Receber"   |
| **E** selecionamos status "Pendente" e período "Este mês"          |
| **QUANDO** clicarmos em "Buscar"                                   |
| **ENTÃO** apenas contas pendentes do mês devem ser exibidas        |

| **Critérios de aceitação**                     |
| :--------------------------------------------- |
| O resultado deve respeitar todos os filtros.   |

---

### Caso de Teste 03: Lançar conta sem valor.

| ID       | Descrição |
| :------- | :-------- |
| C14-CT03 | O sistema deve bloquear conta sem valor. |

| **Pré-condições**                                     |
| :---------------------------------------------------- |
| O cliente "Cliente Teste QA" deve estar cadastrado.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Contas a Receber"              |
| **E** clicamos em "Nova Conta"                                                |
| **E** deixamos o valor em branco                                              |
| **QUANDO** clicarmos em "Salvar"                                              |
| **ENTÃO** mensagens de validação devem ser exibidas nos campos obrigatórios   |

| **Critérios de aceitação**                 |
| :----------------------------------------- |
| Nenhuma conta deve ser criada sem valor.   |
