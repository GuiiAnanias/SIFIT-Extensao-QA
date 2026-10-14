## Cenário 10: Grupos musculares e objetivos de treino.

### Caso de Teste 01: Cadastrar grupo muscular.

| ID       | Descrição |
| :------- | :-------- |
| C10-CT01 | O sistema deve cadastrar um grupo muscular. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                  |
| :-------------------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Grupos Musculares"                    |
| **E** clicamos em "Cadastrar grupo"                                         |
| **E** preenchemos o nome "Grupo Teste QA" e o tipo de membro "Superiores"   |
| **QUANDO** clicarmos em "Salvar"                                            |
| **ENTÃO** o grupo deve aparecer na listagem com o tipo informado            |

| **Critérios de aceitação**               |
| :--------------------------------------- |
| O grupo deve ser listado corretamente.   |

---

### Caso de Teste 02: Filtrar grupos por tipo de membro.

| ID       | Descrição |
| :------- | :-------- |
| C10-CT02 | O filtro deve exibir apenas o tipo escolhido. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                      |
| :-------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Grupos Musculares"        |
| **E** selecionamos o tipo "Inferiores"                          |
| **QUANDO** clicarmos em "Buscar"                                |
| **ENTÃO** apenas grupos do tipo Inferiores devem ser exibidos   |

| **Critérios de aceitação**                  |
| :------------------------------------------ |
| O filtro deve respeitar o tipo de membro.   |

---

### Caso de Teste 03: Cadastrar objetivo de treino sem nome.

| ID       | Descrição |
| :------- | :-------- |
| C10-CT03 | O sistema deve bloquear objetivo sem nome. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Objetivos Treino"                       |
| **E** clicamos em "Novo Objetivo"                                             |
| **E** deixamos o nome do objetivo em branco                                   |
| **QUANDO** clicarmos em "Salvar"                                              |
| **ENTÃO** mensagens de validação devem ser exibidas nos campos obrigatórios   |

| **Critérios de aceitação**         |
| :--------------------------------- |
| Nenhum objetivo deve ser criado.   |
