## Cenário 26: Fichas, modelos e perguntas de anamnese.

### Caso de Teste 01: Criar ficha de anamnese.

| ID       | Descrição |
| :------- | :-------- |
| C26-CT01 | O sistema deve criar uma anamnese para o cliente. |

| **Pré-condições**                                                                            |
| :------------------------------------------------------------------------------------------- |
| O cliente "Cliente Teste QA" deve estar cadastrado. Deve existir modelo de anamnese ativo.   |

| **Passos**                                                        |
| :---------------------------------------------------------------- |
| **DADO** que acessamos "Saúde > Fichas Anamnese"                  |
| **E** clicamos em "Nova Anamnese"                                 |
| **E** preenchemos o cliente de teste e um modelo                  |
| **QUANDO** clicarmos em "Salvar"                                  |
| **ENTÃO** a ficha deve aparecer na listagem com status Pendente   |

| **Critérios de aceitação**                       |
| :----------------------------------------------- |
| A ficha deve ser vinculada ao cliente correto.   |

---

### Caso de Teste 02: Cadastrar pergunta de anamnese.

| ID       | Descrição |
| :------- | :-------- |
| C26-CT02 | O sistema deve cadastrar uma pergunta. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                              |
| :-------------------------------------------------------------------------------------- |
| **DADO** que acessamos "Saúde > Perguntas"                                              |
| **E** clicamos em "Nova Pergunta"                                                       |
| **E** preenchemos o nome, a pergunta "Pratica atividade física?" e o tipo de resposta   |
| **QUANDO** clicarmos em "Salvar"                                                        |
| **ENTÃO** a pergunta deve aparecer na listagem com status Ativo                         |

| **Critérios de aceitação**     |
| :----------------------------- |
| A pergunta deve ser listada.   |

---

### Caso de Teste 03: Visualizar preview do modelo.

| ID       | Descrição |
| :------- | :-------- |
| C26-CT03 | O sistema deve mostrar como o modelo aparece para o aluno. |

| **Pré-condições**                  |
| :--------------------------------- |
| Deve existir modelo de anamnese.   |

| **Passos**                                            |
| :---------------------------------------------------- |
| **DADO** que acessamos "Saúde > Modelos"              |
| **QUANDO** clicarmos em "Preview" em um modelo        |
| **ENTÃO** as perguntas do modelo devem ser exibidas   |

| **Critérios de aceitação**                             |
| :----------------------------------------------------- |
| O preview deve mostrar todas as perguntas do modelo.   |
