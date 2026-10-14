## Cenário 27: Inteligência e automação.

### Caso de Teste 01: Consultar central de automações.

| ID       | Descrição |
| :------- | :-------- |
| C27-CT01 | A tela deve listar as automações ativas e disponíveis. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                                   |
| :------------------------------------------------------------------------------------------- |
| **DADO** que acessamos "Inteligência > Inteligência & Automação"                             |
| **QUANDO** a tela for carregada                                                              |
| **ENTÃO** devem ser exibidas Automações ativas, Automações disponíveis e Atividade recente   |

| **Critérios de aceitação**           |
| :----------------------------------- |
| Os blocos devem carregar sem erro.   |

---

### Caso de Teste 02: Consultar resultados por período.

| ID       | Descrição |
| :------- | :-------- |
| C27-CT02 | Os resultados devem ser filtrados pelo período. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                             |
| :--------------------------------------------------------------------- |
| **DADO** que acessamos "Inteligência > Resultados IA"                  |
| **QUANDO** clicarmos em "Hoje", "Últimos 7 dias" e "Últimos 30 dias"   |
| **ENTÃO** os resultados devem ser atualizados para cada período        |

| **Critérios de aceitação**                   |
| :------------------------------------------- |
| Os valores devem mudar conforme o período.   |

---

### Caso de Teste 03: Abrir configuração de automação.

| ID       | Descrição |
| :------- | :-------- |
| C27-CT03 | O sistema deve abrir a configuração sem salvar alterações. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                         |
| :----------------------------------------------------------------- |
| **DADO** que acessamos "Inteligência > Inteligência & Automação"   |
| **QUANDO** clicarmos em "Configurar" em uma automação              |
| **ENTÃO** a tela de configuração deve abrir                        |
| **E** ao cancelar nada deve ser alterado                           |

| **Critérios de aceitação**                                             |
| :--------------------------------------------------------------------- |
| A configuração deve abrir e o cancelamento não deve gravar mudanças.   |
