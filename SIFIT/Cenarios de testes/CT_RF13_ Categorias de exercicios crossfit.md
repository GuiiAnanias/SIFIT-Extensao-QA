## Cenário 13: Categorias de exercícios crossfit.

### Caso de Teste 01: Cadastrar categoria.

| ID       | Descrição |
| :------- | :-------- |
| C13-CT01 | O sistema deve cadastrar uma categoria de crossfit. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                            |
| :-------------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Categorias Crossfit"            |
| **E** clicamos em "Nova Categoria"                                    |
| **E** preenchemos o nome "Categoria Teste QA"                         |
| **QUANDO** clicarmos em "Salvar"                                      |
| **ENTÃO** a categoria deve aparecer na listagem com data de criação   |

| **Critérios de aceitação**      |
| :------------------------------ |
| A categoria deve ser listada.   |

---

### Caso de Teste 02: Editar categoria.

| ID       | Descrição |
| :------- | :-------- |
| C13-CT02 | O sistema deve permitir alterar o nome da categoria. |

| **Pré-condições**                    |
| :----------------------------------- |
| Deve existir a categoria de teste.   |

| **Passos**                                                                  |
| :-------------------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Categorias Crossfit"                  |
| **E** clicamos em "Editar" na categoria de teste                            |
| **E** alteramos o nome para "Categoria Teste QA 2"                          |
| **QUANDO** clicarmos em "Salvar"                                            |
| **ENTÃO** o novo nome deve aparecer e a coluna "Atualizado em" deve mudar   |

| **Critérios de aceitação**      |
| :------------------------------ |
| A alteração deve ser gravada.   |

---

### Caso de Teste 03: Buscar categoria por nome.

| ID       | Descrição |
| :------- | :-------- |
| C13-CT03 | A busca deve retornar a categoria pesquisada. |

| **Pré-condições**                    |
| :----------------------------------- |
| Deve existir a categoria de teste.   |

| **Passos**                                                   |
| :----------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Categorias Crossfit"   |
| **E** preenchemos "Teste QA" em "Nome"                       |
| **QUANDO** clicarmos em "Buscar"                             |
| **ENTÃO** apenas a categoria de teste deve ser exibida       |

| **Critérios de aceitação**             |
| :------------------------------------- |
| O resultado deve respeitar o filtro.   |
