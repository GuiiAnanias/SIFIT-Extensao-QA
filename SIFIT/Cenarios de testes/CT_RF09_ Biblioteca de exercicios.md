## Cenário 09: Biblioteca de exercícios.

### Caso de Teste 01: Adicionar exercício.

| ID       | Descrição |
| :------- | :-------- |
| C09-CT01 | O sistema deve cadastrar um exercício em um grupo muscular. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Exercícios"                             |
| **E** clicamos em "Adicionar"                                                 |
| **E** preenchemos o nome "Exercício Teste QA" e um grupo muscular             |
| **QUANDO** clicarmos em "Salvar"                                              |
| **ENTÃO** o exercício deve aparecer na biblioteca dentro do grupo escolhido   |

| **Critérios de aceitação**                       |
| :----------------------------------------------- |
| O exercício deve ser exibido no grupo correto.   |

---

### Caso de Teste 02: Adicionar exercício sem nome.

| ID       | Descrição |
| :------- | :-------- |
| C09-CT02 | O sistema deve bloquear exercício sem nome. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Exercícios"                             |
| **E** clicamos em "Adicionar"                                                 |
| **E** deixamos o nome do exercício em branco                                  |
| **QUANDO** clicarmos em "Salvar"                                              |
| **ENTÃO** mensagens de validação devem ser exibidas nos campos obrigatórios   |

| **Critérios de aceitação**          |
| :---------------------------------- |
| Nenhum exercício deve ser criado.   |

---

### Caso de Teste 03: Visualizar exercício.

| ID       | Descrição |
| :------- | :-------- |
| C09-CT03 | O sistema deve exibir os dados do exercício. |

| **Pré-condições**                    |
| :----------------------------------- |
| Deve existir exercício cadastrado.   |

| **Passos**                                             |
| :----------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Exercícios"      |
| **QUANDO** clicarmos em "Visualizar" em um exercício   |
| **ENTÃO** os dados do exercício devem ser exibidos     |

| **Critérios de aceitação**                 |
| :----------------------------------------- |
| Os dados devem corresponder ao cadastro.   |
