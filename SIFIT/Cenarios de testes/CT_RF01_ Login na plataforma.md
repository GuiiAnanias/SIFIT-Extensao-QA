## Cenário 01: Login na plataforma.

### Caso de Teste 01: Login com credenciais válidas.

| ID       | Descrição |
| :------- | :-------- |
| C01-CT01 | O login será realizado com usuário e senha válidos. |

| **Pré-condições**                                                       |
| :---------------------------------------------------------------------- |
| As credenciais de teste fornecidas pelo professor devem estar ativas.   |

| **Passos**                                                                         |
| :--------------------------------------------------------------------------------- |
| **DADO** que estamos na página de login do SIFIT                                   |
| **E** preenchemos o usuário válido no campo "Login"                                |
| **E** preenchemos a senha válida no campo "Senha"                                  |
| **QUANDO** clicarmos no botão "Entrar"                                             |
| **ENTÃO** seremos redirecionados para a Página Inicial com a saudação ao usuário   |

| **Critérios de aceitação**                                            |
| :-------------------------------------------------------------------- |
| O redirecionamento para a Página Inicial deve ocorrer corretamente.   |

---

### Caso de Teste 02: Tentativa de login com senha incorreta.

| ID       | Descrição |
| :------- | :-------- |
| C01-CT02 | O login falhará quando a senha for inválida. |

| **Pré-condições**                             |
| :-------------------------------------------- |
| O usuário de teste deve existir no sistema.   |

| **Passos**                                                                     |
| :----------------------------------------------------------------------------- |
| **DADO** que estamos na página de login do SIFIT                               |
| **E** preenchemos o usuário válido no campo "Login"                            |
| **E** preenchemos "senhaerrada" no campo "Senha"                               |
| **QUANDO** clicarmos no botão "Entrar"                                         |
| **ENTÃO** uma mensagem de erro será exibida e continuaremos na tela de login   |

| **Critérios de aceitação**                                               |
| :----------------------------------------------------------------------- |
| A mensagem de erro deve ser exibida e o acesso não deve ser concedido.   |

---

### Caso de Teste 03: Tentativa de login com campos em branco.

| ID       | Descrição |
| :------- | :-------- |
| C01-CT03 | O login falhará quando os campos estiverem em branco. |

| **Pré-condições**   |
| :------------------ |
| Nenhuma.            |

| **Passos**                                                  |
| :---------------------------------------------------------- |
| **DADO** que estamos na página de login do SIFIT            |
| **E** deixamos os campos "Login" e "Senha" em branco        |
| **QUANDO** clicarmos no botão "Entrar"                      |
| **ENTÃO** o sistema deve sinalizar os campos obrigatórios   |

| **Critérios de aceitação**                                   |
| :----------------------------------------------------------- |
| Os campos obrigatórios devem exibir mensagem de validação.   |
