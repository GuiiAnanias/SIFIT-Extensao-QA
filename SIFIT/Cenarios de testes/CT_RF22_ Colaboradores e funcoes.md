## Cenário 22: Colaboradores e funções.

### Caso de Teste 01: Pesquisar colaborador.

| ID       | Descrição |
| :------- | :-------- |
| C22-CT01 | A busca deve retornar o colaborador pelo nome. |

| **Pré-condições**                      |
| :------------------------------------- |
| Deve existir colaborador cadastrado.   |

| **Passos**                                                                |
| :------------------------------------------------------------------------ |
| **DADO** que acessamos "Gestão > Colaboradores"                           |
| **E** preenchemos parte do nome de um colaborador                         |
| **QUANDO** clicarmos em "Buscar"                                          |
| **ENTÃO** apenas colaboradores com o nome pesquisado devem ser exibidos   |

| **Critérios de aceitação**             |
| :------------------------------------- |
| O resultado deve respeitar o filtro.   |

---

### Caso de Teste 02: Cadastrar função.

| ID       | Descrição |
| :------- | :-------- |
| C22-CT02 | O sistema deve cadastrar uma nova função. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                      |
| :-------------------------------------------------------------- |
| **DADO** que acessamos "Gestão > Funções"                       |
| **E** clicamos em "Nova Função"                                 |
| **E** preenchemos o nome "Função Teste QA" e o tipo "Interno"   |
| **QUANDO** clicarmos em "Salvar"                                |
| **ENTÃO** a função deve aparecer na listagem                    |

| **Critérios de aceitação**                        |
| :------------------------------------------------ |
| A função deve ser listada com o tipo informado.   |

---

### Caso de Teste 03: Consultar permissões da função.

| ID       | Descrição |
| :------- | :-------- |
| C22-CT03 | O sistema deve exibir as permissões de uma função. |

| **Pré-condições**                 |
| :-------------------------------- |
| Deve existir função cadastrada.   |

| **Passos**                                                   |
| :----------------------------------------------------------- |
| **DADO** que acessamos "Gestão > Funções"                    |
| **QUANDO** clicarmos em "Permissões" em uma função           |
| **ENTÃO** a lista de permissões da função deve ser exibida   |

| **Critérios de aceitação**            |
| :------------------------------------ |
| As permissões devem abrir sem erro.   |
