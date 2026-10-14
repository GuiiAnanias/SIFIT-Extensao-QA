## Cenário 04: Consulta de Presenças.

### Caso de Teste 01: Filtrar presenças por período.

| ID       | Descrição |
| :------- | :-------- |
| C04-CT01 | A tela deve filtrar pelo período escolhido. |

| **Pré-condições**                   |
| :---------------------------------- |
| Deve existir check-in registrado.   |

| **Passos**                                                               |
| :----------------------------------------------------------------------- |
| **DADO** que acessamos "Principal > Presenças"                           |
| **QUANDO** clicarmos em "Hoje", "Esta semana" e "Este mês"               |
| **ENTÃO** a lista deve ser atualizada com os registros de cada período   |

| **Critérios de aceitação**                                |
| :-------------------------------------------------------- |
| Os registros devem corresponder ao período selecionado.   |

---

### Caso de Teste 02: Buscar presenças de um cliente.

| ID       | Descrição |
| :------- | :-------- |
| C04-CT02 | A busca deve retornar as presenças do cliente informado. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O cliente de teste deve ter check-in.   |

| **Passos**                                                         |
| :----------------------------------------------------------------- |
| **DADO** que acessamos "Principal > Presenças"                     |
| **E** digitamos "Cliente Teste QA" em "Buscar por cliente"         |
| **QUANDO** clicarmos em "Buscar"                                   |
| **ENTÃO** devem aparecer apenas as presenças do cliente de teste   |

| **Critérios de aceitação**                 |
| :----------------------------------------- |
| A busca deve respeitar o nome informado.   |

---

### Caso de Teste 03: Buscar cliente sem presenças.

| ID       | Descrição |
| :------- | :-------- |
| C04-CT03 | O sistema deve informar quando não há resultados. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                               |
| :----------------------------------------------------------------------- |
| **DADO** que acessamos "Principal > Presenças"                           |
| **E** digitamos "zzzz" em "Buscar por cliente"                           |
| **QUANDO** clicarmos em "Buscar"                                         |
| **ENTÃO** o sistema deve exibir mensagem de nenhum registro encontrado   |

| **Critérios de aceitação**     |
| :----------------------------- |
| A tela não deve exibir erro.   |
