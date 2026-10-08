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

* Autenticação de usuário
* Página inicial e dashboard
* Check-in e presenças
* Clientes
* Matrículas
* Avaliações físicas
* Treinamento
* Financeiro
* Comercial
* Relatórios
* Gestão
* Anamnese

**Excluído:**

* Recuperação de senha e integrações de pagamento
* Configurações do sistema (afetam o ambiente de toda a turma)
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
| Planejamento de Testes      | 07/10/2026  | 07/10/2026 |
| Criação de Casos de Teste   | 11/10/2026  | 11/10/2026 |
| Execução dos Testes Manuais | 11/10/2026  | 11/10/2026 |
| Registro e Report de Bugs   | 11/11/2026  | 11/10/2026 |
| Encerramento e Evidências   | 11/10/2026  | 11/10/2026 |

---

### 9. **Módulos a Serem Testados**

| Código RF | Módulo                     | Prioridade |
| --------- | -------------------------- | ---------- |
| RF01      | Login                      | Alta       |
| RF02      | Página Inicial / Dashboard | Média      |
| RF03      | Check-in e Presenças       | Alta       |
| RF04      | Clientes                   | Alta       |
| RF05      | Matrículas                 | Alta       |
| RF06      | Avaliações Físicas         | Média      |
| RF07      | Treinamento                | Média      |
| RF08      | Financeiro                 | Alta       |
| RF09      | Comercial                  | Média      |
| RF10      | Relatórios                 | Média      |
| RF11      | Gestão                     | Baixa      |
| RF12      | Anamnese                   | Baixa      |

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