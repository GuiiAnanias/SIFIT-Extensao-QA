## **Plano de Testes - SIFIT**

### 1. **Identificação**

* **Nome do Projeto**: SIFIT - Sistema para Academias
* **Versão Avaliada**: Ambiente disponibilizado pelo professor
* **Ambiente de Testes**: [https://sifit.centrion.com.br](https://sifit.centrion.com.br)
* **Tipo de Teste**: Teste Funcional Manual
* **Data do Documento**: 08/10/2026
* **Responsável**: Guilherme Calixto

---

### 2. **Objetivo**

Realizar a verificação manual dos principais requisitos funcionais do SIFIT, com foco nos fluxos mais usados no dia a dia de uma academia, nas mensagens de erro e no comportamento esperado das telas.

---

### 3. **Escopo**

**Incluído:**

* Todos os módulos do menu do sistema: Principal, Operação da Academia, Treinamento, Financeiro, Comercial, Gestão, Saúde, Inteligência e Configurações (29 requisitos, ver Análise de Requisitos)

**Excluído:**

* Recuperação de senha
* Ações que movimentam dinheiro ou enviam mensagens reais (saque e cobrança no Pagar.me, cobrança pelo WhatsApp, executar automações)
* Salvar alterações em Configurações (afetam o ambiente de toda a turma)
* Testes em dispositivos móveis
* Testes de performance ou carga

---

### 4. **Ferramentas Utilizadas**

* Navegador Google Chrome
* Ferramentas de inspeção do navegador (DevTools)
* Extensão Jam (gravação das evidências)
* MySQL Workbench (consulta ao banco)

---

### 5. **Técnicas de Teste**

* Particionamento de equivalência
* Análise de valor limite
* Caminho feliz (Happy Path)
* Testes negativos
* Testes exploratórios

---

### 6. **Critérios de Aceitação**

* Todos os casos de teste devem passar com sucesso, conforme o resultado esperado.
* Nenhuma falha crítica deve estar presente em funcionalidades principais.
* Mensagens de erro e validações devem ser consistentes.

---

### 7. **Critérios de Saída (Exit Criteria)**

* Todos os testes do escopo foram executados.
* Falhas foram registradas, analisadas e reexecutadas se necessário.
* Documentação de evidências de sucesso e falhas está completa.

---

### 8. **Cronograma Estimado**

| Atividade                   | Data Início | Data Fim   |
| --------------------------- | ----------- | ---------- |
| Planejamento de Testes      | 08/10/2026  | 08/10/2026 |
| Criação de Casos de Teste   | xx/xx/2026  | xx/xx/2026 |
| Execução dos Testes Manuais | xx/xx/2026  | xx/xx/2026 |
| Registro e Report de Bugs   | xx/xx/2026  | xx/xx/2026 |
| Encerramento e Evidências   | xx/xx/2026  | xx/xx/2026 |

---

### 9. **Módulos a Serem Testados**

| Código RF | Módulo                             | Prioridade |
| --------- | ---------------------------------- | ---------- |
| RF01      | Login                              | Alta       |
| RF02      | Página Inicial / Dashboard         | Média      |
| RF03      | Check-in                           | Alta       |
| RF04      | Presenças                          | Média      |
| RF05      | Clientes                           | Alta       |
| RF06      | Matrículas                         | Alta       |
| RF07      | Avaliações Físicas                 | Média      |
| RF08      | Fichas de Treino                   | Média      |
| RF09      | Exercícios                         | Baixa      |
| RF10      | Grupos Musculares / Objetivos      | Baixa      |
| RF11      | Turmas e Grupos                    | Média      |
| RF12      | SifitBox                           | Média      |
| RF13      | Categorias Crossfit                | Baixa      |
| RF14      | Contas a Receber                   | Alta       |
| RF15      | Contas a Pagar                     | Alta       |
| RF16      | Caixas                             | Alta       |
| RF17      | Despesas Fixas                     | Média      |
| RF18      | Pagar.me                           | Média      |
| RF19      | Relatórios                         | Média      |
| RF20      | Prospecção                         | Média      |
| RF21      | Planos e Formas de Pagamento       | Média      |
| RF22      | Colaboradores e Funções            | Baixa      |
| RF23      | Fornecedores e Tipos de Documentos | Baixa      |
| RF24      | Atividades, Pontuação e Produtos   | Baixa      |
| RF25      | Enquetes                           | Baixa      |
| RF26      | Anamnese                           | Média      |
| RF27      | Inteligência e Automação           | Baixa      |
| RF28      | Aplicativo                         | Baixa      |
| RF29      | Configurações                      | Baixa      |

---

### 10. **Gestão de Defeitos**

* Bugs serão documentados com:

  * Título
  * Descrição
  * Passos para reproduzir
  * Evidência (print ou vídeo)
  * Gravidade (Crítica, Alta, Média, Baixa)

---

### 11. **Riscos Identificados**

| Risco                                     | Impacto | Mitigação                                  |
| ----------------------------------------- | ------- | ------------------------------------------ |
| Sistema fora do ar                        | Alto    | Tentar novamente após intervalo            |
| Ambiente usado pela turma toda            | Médio   | Identificar os registros criados no teste  |
| Testes limitados a um único usuário       | Médio   | Documentar esse limite no escopo           |

---

### 12. **Entregáveis**

* Plano de Testes (.md)
* Casos de Teste (.md)
* Evidências de Execução (prints e vídeos por RF)
* Registro de Bugs (se houver)
* Relatório Final de Execução
