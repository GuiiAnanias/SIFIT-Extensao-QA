## Cenário 28: Aplicativo, notificações e postagens.

### Caso de Teste 01: Consultar notificações.

| ID       | Descrição |
| :------- | :-------- |
| C28-CT01 | A tela deve listar as notificações enviadas. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                              |
| :------------------------------------------------------ |
| **DADO** que acessamos "Configurações > Aplicativo"     |
| **QUANDO** clicarmos em "Ver todas as notificações"     |
| **ENTÃO** a lista deve exibir Código, Mensagem e Data   |

| **Critérios de aceitação**     |
| :----------------------------- |
| A lista deve abrir sem erro.   |

---

### Caso de Teste 02: Filtrar postagens pendentes.

| ID       | Descrição |
| :------- | :-------- |
| C28-CT02 | O filtro deve exibir apenas postagens pendentes. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                          |
| :------------------------------------------------------------------ |
| **DADO** que acessamos "Configurações > Aplicativo"                 |
| **QUANDO** clicarmos em "Só pendentes"                              |
| **ENTÃO** apenas postagens com status pendente devem ser exibidas   |

| **Critérios de aceitação**             |
| :------------------------------------- |
| O resultado deve respeitar o status.   |

---

### Caso de Teste 03: Visualizar denúncia.

| ID       | Descrição |
| :------- | :-------- |
| C28-CT03 | O sistema deve exibir os dados de uma denúncia. |

| **Pré-condições**                   |
| :---------------------------------- |
| Deve existir denúncia registrada.   |

| **Passos**                                                                  |
| :-------------------------------------------------------------------------- |
| **DADO** que acessamos "Configurações > Aplicativo"                         |
| **QUANDO** clicarmos em "Visualizar" em uma denúncia                        |
| **ENTÃO** devem aparecer a postagem denunciada, o motivo e quem denunciou   |

| **Critérios de aceitação**              |
| :-------------------------------------- |
| Os dados devem ser exibidos sem erro.   |
