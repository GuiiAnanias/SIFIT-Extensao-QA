## Cenário 20: Prospecção de leads.

### Caso de Teste 01: Adicionar lead.

| ID       | Descrição |
| :------- | :-------- |
| C20-CT01 | O sistema deve registrar um lead no início do funil. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                 |
| :--------------------------------------------------------- |
| **DADO** que acessamos "Comercial > Prospecção"            |
| **E** clicamos em "Adicionar Lead"                         |
| **E** preenchemos o nome "Lead Teste QA" e um telefone     |
| **QUANDO** clicarmos em "Salvar"                           |
| **ENTÃO** o lead deve aparecer no estágio "Novo Contato"   |

| **Critérios de aceitação**                       |
| :----------------------------------------------- |
| O lead deve ser listado com a data de criação.   |

---

### Caso de Teste 02: Filtrar leads por estágio.

| ID       | Descrição |
| :------- | :-------- |
| C20-CT02 | O filtro deve exibir apenas o estágio escolhido. |

| **Pré-condições**               |
| :------------------------------ |
| Deve existir lead cadastrado.   |

| **Passos**                                                                                        |
| :------------------------------------------------------------------------------------------------ |
| **DADO** que acessamos "Comercial > Prospecção"                                                   |
| **QUANDO** selecionarmos o estágio "Novo Contato"                                                 |
| **ENTÃO** apenas leads nesse estágio devem ser exibidos e "Limpar" deve voltar a lista completa   |

| **Critérios de aceitação**              |
| :-------------------------------------- |
| O filtro deve funcionar corretamente.   |

---

### Caso de Teste 03: Adicionar lead sem nome.

| ID       | Descrição |
| :------- | :-------- |
| C20-CT03 | O sistema deve bloquear lead sem nome. |

| **Pré-condições**                       |
| :-------------------------------------- |
| O usuário deve estar logado no SIFIT.   |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que acessamos "Comercial > Prospecção"                               |
| **E** clicamos em "Adicionar Lead"                                            |
| **E** deixamos o nome em branco                                               |
| **QUANDO** clicarmos em "Salvar"                                              |
| **ENTÃO** mensagens de validação devem ser exibidas nos campos obrigatórios   |

| **Critérios de aceitação**     |
| :----------------------------- |
| Nenhum lead deve ser criado.   |
