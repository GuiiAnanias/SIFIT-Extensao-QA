## Cenário 05: Gestão de clientes.

### Caso de Teste 01: Cadastrar cliente com dados obrigatórios.

| ID       | Descrição |
| :------- | :-------- |
| C05-CT01 | O sistema deve cadastrar um cliente com os campos obrigatórios. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                             |
| :------------------------------------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Clientes"                               |
| **E** clicamos em "Novo Cliente"                                                       |
| **E** preenchemos Nome "Cliente Teste QA", Status "Ativo", Sexo e Data de Nascimento   |
| **QUANDO** clicarmos em "Cadastrar Cliente"                                            |
| **ENTÃO** o cliente deve aparecer na listagem                                          |

| **Critérios de aceitação**                                     |
| :------------------------------------------------------------- |
| O cliente deve ser listado com código gerado e status Ativo.   |

---

### Caso de Teste 02: Cadastrar cliente sem campos obrigatórios.

| ID       | Descrição |
| :------- | :-------- |
| C05-CT02 | O sistema deve bloquear o cadastro sem Nome, Status, Sexo e Data de Nascimento. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Clientes"                      |
| **E** clicamos em "Novo Cliente"                                              |
| **E** deixamos Nome, Status, Sexo e Data de Nascimento em branco              |
| **QUANDO** clicarmos em "Cadastrar Cliente"                                   |
| **ENTÃO** mensagens de validação devem ser exibidas nos campos obrigatórios   |

| **Critérios de aceitação**        |
| :-------------------------------- |
| Nenhum cliente deve ser criado.   |

---

### Caso de Teste 03: Pesquisar cliente cadastrado.

| ID       | Descrição |
| :------- | :-------- |
| C05-CT03 | A busca deve retornar o cliente pelo nome. |

| **Pré-condições**                                     |
| :---------------------------------------------------- |
| O cliente "Cliente Teste QA" deve estar cadastrado.   |

| **Passos**                                                 |
| :--------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Clientes"   |
| **E** preenchemos "Teste QA" no campo "Nome"               |
| **QUANDO** clicarmos em "Buscar"                           |
| **ENTÃO** a listagem deve exibir o cliente de teste        |

| **Critérios de aceitação**                                       |
| :--------------------------------------------------------------- |
| O resultado deve conter apenas clientes com o nome pesquisado.   |
