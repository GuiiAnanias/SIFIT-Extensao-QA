## Cenário 08: Fichas de treino e modelos de ficha.

### Caso de Teste 01: Cadastrar ficha de treino.

| ID       | Descrição |
| :------- | :-------- |
| C08-CT01 | O sistema deve criar uma ficha para o cliente. |

| **Pré-condições**                                     |
| :---------------------------------------------------- |
| O cliente "Cliente Teste QA" deve estar cadastrado.   |

| **Passos**                                                      |
| :-------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Ficha de Treino"          |
| **E** clicamos em "Cadastrar Ficha"                             |
| **E** preenchemos o cliente de teste, as datas e um exercício   |
| **QUANDO** clicarmos em "Salvar"                                |
| **ENTÃO** a ficha deve aparecer na listagem com status Ativo    |

| **Critérios de aceitação**                     |
| :--------------------------------------------- |
| A ficha deve ser vinculada ao aluno correto.   |

---

### Caso de Teste 02: Filtrar fichas por status.

| ID       | Descrição |
| :------- | :-------- |
| C08-CT02 | O filtro deve exibir apenas fichas do status escolhido. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                                          |
| :-------------------------------------------------------------------------------------------------- |
| **DADO** que acessamos "Treinamento > Ficha de Treino"                                              |
| **E** selecionamos o status "Ativo"                                                                 |
| **QUANDO** clicarmos em "Buscar"                                                                    |
| **ENTÃO** apenas fichas ativas devem ser exibidas e "Limpar filtros" deve voltar a lista completa   |

| **Critérios de aceitação**                         |
| :------------------------------------------------- |
| O filtro e a limpeza de filtros devem funcionar.   |

---

### Caso de Teste 03: Consultar modelos de ficha.

| ID       | Descrição |
| :------- | :-------- |
| C08-CT03 | A tela deve listar os modelos de ficha cadastrados. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                                                    |
| :------------------------------------------------------------------------------------------------------------ |
| **DADO** que acessamos "Configurações > Modelo Ficha"                                                         |
| **QUANDO** a tela for carregada                                                                               |
| **ENTÃO** devem ser exibidos os indicadores Modelos, Criadores, Listados e Sem Criador e a lista de modelos   |

| **Critérios de aceitação**                                   |
| :----------------------------------------------------------- |
| Os totais dos indicadores devem bater com a lista exibida.   |
