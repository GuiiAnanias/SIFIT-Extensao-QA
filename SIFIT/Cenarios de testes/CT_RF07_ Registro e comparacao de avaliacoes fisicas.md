## Cenário 07: Registro e comparação de avaliações físicas.

### Caso de Teste 01: Cadastrar avaliação física.

| ID       | Descrição |
| :------- | :-------- |
| C07-CT01 | O sistema deve registrar uma avaliação para o cliente. |

| **Pré-condições**                                     |
| :---------------------------------------------------- |
| O cliente "Cliente Teste QA" deve estar cadastrado.   |

| **Passos**                                                       |
| :--------------------------------------------------------------- |
| **DADO** que acessamos "Operação da Academia > Avaliações"       |
| **E** clicamos em "Cadastrar Avaliação"                          |
| **E** preenchemos o cliente de teste, a data/hora e o personal   |
| **QUANDO** clicarmos em "Salvar"                                 |
| **ENTÃO** a avaliação deve aparecer na listagem                  |

| **Critérios de aceitação**                              |
| :------------------------------------------------------ |
| A avaliação deve ser listada com os dados informados.   |

---

### Caso de Teste 02: Visualizar avaliação.

| ID       | Descrição |
| :------- | :-------- |
| C07-CT02 | O sistema deve exibir os dados de uma avaliação. |

| **Pré-condições**                             |
| :-------------------------------------------- |
| Deve existir avaliação do cliente de teste.   |

| **Passos**                                                              |
| :---------------------------------------------------------------------- |
| **DADO** que estamos na listagem de Avaliações                          |
| **QUANDO** clicarmos em "Visualizar" na avaliação do cliente de teste   |
| **ENTÃO** os dados da avaliação devem ser exibidos                      |

| **Critérios de aceitação**                           |
| :--------------------------------------------------- |
| Os dados exibidos devem ser os mesmos do cadastro.   |

---

### Caso de Teste 03: Comparar avaliações.

| ID       | Descrição |
| :------- | :-------- |
| C07-CT03 | O sistema deve comparar duas avaliações do mesmo aluno. |

| **Pré-condições**                              |
| :--------------------------------------------- |
| O cliente de teste deve ter duas avaliações.   |

| **Passos**                                                       |
| :--------------------------------------------------------------- |
| **DADO** que estamos na listagem de Avaliações                   |
| **QUANDO** clicarmos em "Comparação" para o cliente de teste     |
| **ENTÃO** o sistema deve exibir a evolução entre as avaliações   |

| **Critérios de aceitação**                                         |
| :----------------------------------------------------------------- |
| A comparação deve usar apenas avaliações do cliente selecionado.   |
