## Cenário 11: Turmas e grupos.

### Caso de Teste 01: Cadastrar turma.

| ID       | Descrição |
| :------- | :-------- |
| C11-CT01 | O sistema deve cadastrar uma turma com horário e dias. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                |
| :------------------------------------------------------------------------ |
| **DADO** que acessamos "Treinamento > Turmas"                             |
| **E** clicamos em "Cadastrar Turma"                                       |
| **E** preenchemos o nome "Turma Teste QA", o plano, o horário e os dias   |
| **QUANDO** clicarmos em "Salvar"                                          |
| **ENTÃO** a turma deve aparecer na listagem com status Ativo              |

| **Critérios de aceitação**                          |
| :-------------------------------------------------- |
| A turma deve ser listada com os dados informados.   |

---

### Caso de Teste 02: Cadastrar turma sem nome.

| ID       | Descrição |
| :------- | :-------- |
| C11-CT02 | O sistema deve bloquear turma sem nome. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Turmas"                                 |
| **E** clicamos em "Cadastrar Turma"                                           |
| **E** deixamos o nome da turma em branco                                      |
| **QUANDO** clicarmos em "Salvar"                                              |
| **ENTÃO** mensagens de validação devem ser exibidas nos campos obrigatórios   |

| **Critérios de aceitação**       |
| :------------------------------- |
| Nenhuma turma deve ser criada.   |

---

### Caso de Teste 03: Filtrar grupos por tipo.

| ID       | Descrição |
| :------- | :-------- |
| C11-CT03 | O filtro deve separar grupos internos e externos. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                   |
| :----------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Grupos"                |
| **QUANDO** selecionarmos o tipo "Interno"                    |
| **ENTÃO** apenas grupos do tipo Interno devem ser exibidos   |

| **Critérios de aceitação**        |
| :-------------------------------- |
| O filtro deve respeitar o tipo.   |
