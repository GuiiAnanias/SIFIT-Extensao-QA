## Cenário 03: Registro de entrada no Check-in.

### Caso de Teste 01: Check-in manual pelo código do cliente.

| ID       | Descrição |
| :------- | :-------- |
| C03-CT01 | O sistema deve registrar a entrada de um cliente ativo. |

| **Pré-condições**                                 |
| :------------------------------------------------ |
| Cliente "Cliente Teste QA" com matrícula ativa.   |

| **Passos**                                                             |
| :--------------------------------------------------------------------- |
| **DADO** que acessamos "Principal > Check-in"                          |
| **E** informamos o código do cliente de teste em "Código do cliente"   |
| **QUANDO** clicarmos em "Realizar check-in"                            |
| **ENTÃO** o cliente deve aparecer em "Presentes agora"                 |

| **Critérios de aceitação**                                             |
| :--------------------------------------------------------------------- |
| O check-in deve ser registrado e o contador de presentes atualizado.   |

---

### Caso de Teste 02: Check-in com código inexistente.

| ID       | Descrição |
| :------- | :-------- |
| C03-CT02 | O sistema não deve registrar entrada para código inexistente. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                           |
| :------------------------------------------------------------------- |
| **DADO** que acessamos "Principal > Check-in"                        |
| **E** informamos "999999" em "Código do cliente"                     |
| **QUANDO** clicarmos em "Realizar check-in"                          |
| **ENTÃO** o sistema deve exibir mensagem de cliente não encontrado   |

| **Critérios de aceitação**             |
| :------------------------------------- |
| Nenhum check-in deve ser registrado.   |

---

### Caso de Teste 03: Filtro de clientes presentes.

| ID       | Descrição |
| :------- | :-------- |
| C03-CT03 | O filtro deve listar apenas quem está presente. |

| **Pré-condições**                          |
| :----------------------------------------- |
| Deve existir check-in registrado no dia.   |

| **Passos**                                                         |
| :----------------------------------------------------------------- |
| **DADO** que acessamos "Principal > Check-in"                      |
| **QUANDO** clicarmos em "Presentes agora"                          |
| **ENTÃO** a lista deve exibir apenas clientes com check-in ativo   |

| **Critérios de aceitação**                            |
| :---------------------------------------------------- |
| O filtro deve respeitar a situação de cada cliente.   |
