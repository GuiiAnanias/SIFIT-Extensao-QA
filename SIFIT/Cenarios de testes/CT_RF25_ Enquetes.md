## Cenário 25: Enquetes.

### Caso de Teste 01: Cadastrar enquete.

| ID       | Descrição |
| :------- | :-------- |
| C25-CT01 | O sistema deve cadastrar uma enquete com pergunta. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                       |
| :--------------------------------------------------------------- |
| **DADO** que acessamos "Gestão > Enquetes"                       |
| **E** clicamos em "Nova Enquete"                                 |
| **E** preenchemos o nome "Enquete Teste QA" e a pergunta         |
| **QUANDO** clicarmos em "Salvar"                                 |
| **ENTÃO** a enquete deve aparecer na listagem com status Ativo   |

| **Critérios de aceitação**    |
| :---------------------------- |
| A enquete deve ser listada.   |

---

### Caso de Teste 02: Filtrar enquetes por status.

| ID       | Descrição |
| :------- | :-------- |
| C25-CT02 | O filtro deve exibir apenas o status escolhido. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                              |
| :------------------------------------------------------ |
| **DADO** que acessamos "Gestão > Enquetes"              |
| **E** selecionamos o status "Inativo"                   |
| **QUANDO** clicarmos em "Buscar"                        |
| **ENTÃO** apenas enquetes inativas devem ser exibidas   |

| **Critérios de aceitação**             |
| :------------------------------------- |
| O resultado deve respeitar o status.   |

---

### Caso de Teste 03: Cadastrar enquete sem pergunta.

| ID       | Descrição |
| :------- | :-------- |
| C25-CT03 | O sistema deve bloquear enquete sem pergunta. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Gestão > Enquetes"                                    |
| **E** clicamos em "Nova Enquete"                                              |
| **E** deixamos a pergunta em branco                                           |
| **QUANDO** clicarmos em "Salvar"                                              |
| **ENTÃO** mensagens de validação devem ser exibidas nos campos obrigatórios   |

| **Critérios de aceitação**         |
| :--------------------------------- |
| Nenhuma enquete deve ser criada.   |
