## Cenário 29: Configurações do sistema.

### Caso de Teste 01: Navegar pelas abas de configuração.

| ID       | Descrição |
| :------- | :-------- |
| C29-CT01 | Cada aba deve abrir suas opções. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                                               |
| :------------------------------------------------------------------------------------------------------- |
| **DADO** que acessamos "Configurações > Configurações"                                                   |
| **QUANDO** clicarmos nas abas Home, Biometria, Avaliação, Aniversário, Pagamento, Integrações e Design   |
| **ENTÃO** cada aba deve exibir suas opções sem erro                                                      |

| **Critérios de aceitação**   |
| :--------------------------- |
| Todas as abas devem abrir.   |

---

### Caso de Teste 02: Cancelar alteração de configuração.

| ID       | Descrição |
| :------- | :-------- |
| C29-CT02 | O botão Cancelar deve descartar mudanças. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                        |
| :------------------------------------------------ |
| **DADO** que estamos na tela de Configurações     |
| **E** alteramos uma opção da aba Home             |
| **QUANDO** clicarmos em "Cancelar"                |
| **ENTÃO** a opção deve voltar ao valor anterior   |

| **Critérios de aceitação**            |
| :------------------------------------ |
| Nenhuma alteração deve ser gravada.   |

---

### Caso de Teste 03: Informar valor negativo em campo numérico.

| ID       | Descrição |
| :------- | :-------- |
| C29-CT03 | Os campos numéricos não devem aceitar valor negativo. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                 |
| :--------------------------------------------------------- |
| **DADO** que estamos na tela de Configurações              |
| **E** informamos "-1" em um campo numérico                 |
| **QUANDO** sairmos do campo                                |
| **ENTÃO** o sistema deve sinalizar o valor como inválido   |

| **Critérios de aceitação**                                                                     |
| :--------------------------------------------------------------------------------------------- |
| O valor negativo não deve ser aceito. Não clicar em Salvar, pois o ambiente é compartilhado.   |
