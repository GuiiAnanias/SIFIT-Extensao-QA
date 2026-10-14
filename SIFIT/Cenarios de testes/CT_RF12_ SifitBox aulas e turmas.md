## Cenário 12: SifitBox aulas e turmas.

### Caso de Teste 01: Gerar aulas por data.

| ID       | Descrição |
| :------- | :-------- |
| C12-CT01 | O sistema deve gerar as aulas do dia a partir das turmas. |

| **Pré-condições**                           |
| :------------------------------------------ |
| Deve existir turma recorrente cadastrada.   |

| **Passos**                                      |
| :---------------------------------------------- |
| **DADO** que acessamos "Principal > SifitBox"   |
| **E** selecionamos a data de amanhã             |
| **QUANDO** clicarmos em "Gerar aulas"           |
| **ENTÃO** as aulas da data devem ser listadas   |

| **Critérios de aceitação**                               |
| :------------------------------------------------------- |
| As aulas geradas devem corresponder às turmas da data.   |

---

### Caso de Teste 02: Cadastrar modalidade.

| ID       | Descrição |
| :------- | :-------- |
| C12-CT02 | O sistema deve cadastrar uma modalidade do Box. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                     |
| :----------------------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Box - Turmas"                            |
| **E** clicamos em "Modalidade"                                                 |
| **E** preenchemos o nome "Modalidade Teste QA", a descrição e o status Ativo   |
| **QUANDO** clicarmos em "Salvar"                                               |
| **ENTÃO** a modalidade deve aparecer na lista de Modalidades                   |

| **Critérios de aceitação**                  |
| :------------------------------------------ |
| A modalidade deve ser listada como Ativa.   |

---

### Caso de Teste 03: Turma recorrente com vagas zeradas.

| ID       | Descrição |
| :------- | :-------- |
| C12-CT03 | O sistema não deve aceitar turma com 0 vagas (valor limite). |

| **Pré-condições**                     |
| :------------------------------------ |
| Deve existir modalidade cadastrada.   |

| **Passos**                                                                 |
| :------------------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Box - Turmas"                        |
| **E** clicamos em "Turma"                                                  |
| **E** preenchemos nome, modalidade, horário, dias e "0" em "Vagas"         |
| **QUANDO** clicarmos em "Salvar"                                           |
| **ENTÃO** o sistema deve exibir mensagem de quantidade de vagas inválida   |

| **Critérios de aceitação**                   |
| :------------------------------------------- |
| Nenhuma turma deve ser criada com 0 vagas.   |
