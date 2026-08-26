## 🔄 Como funciona o Ciclo de Testes na uTest (Test Cycle)

A minha experiência prática com testes é construída participando de ciclos de testes (*Test Cycles*) na plataforma uTest. O fluxo de trabalho segue um processo estruturado de qualidade:

1. **Análise do Overview e Escopo (Scope):** Leitura atenta das instruções do projeto para identificar o que está *In-Scope* (o que deve ser testado, como fluxos de login, pagamento ou UI) e o que está *Out-of-Scope* (o que não deve ser testado).
2. **Setup do Ambiente (Environment):** Configuração do dispositivo (Android, iOS, Web/Navegadores) conforme as especificações solicitadas pelo cliente.
3. **Execução de Casos de Teste e Testes Exploratórios:** Execução dos cenários direcionados (*Test Cases*) ou testes livres (*Exploratory Testing*) para encontrar comportamentos inesperados.
4. **Coleta de Evidências Técnicas:** Utilização do DevTools, Charles Proxy ou gravadores de tela para capturar logs de console, requisições de rede e prints/vídeos demonstrando a falha.
5. **Reporte do Defeito (Bug Report):** Cadastro da falha no padrão exigido (Título objetivo, Passos para Reprodução, Comportamento Esperado vs. Obtido, Severidade e Logs).
6. **Revisão e Aprovacão (TTL & Client Review):** O bug passa pela validação do *Test Team Lead* (TTL) e do cliente antes de ser aprovado no ciclo.




# 📱 Projeto 1: Suíte de Testes Funcionais & Reporte de Bugs

Este projeto documenta o planejamento, a execução de casos de teste manuais e a identificação de falhas funcionais em aplicações Web/Mobile, com base em cenários práticos e execuções na plataforma **uTest**.

---

## 🎯 Objetivo dos Testes
Validar os fluxos críticos da aplicação (como navegação, cadastro/login, interações da interface e regras de negócio), garantindo que o sistema responda conforme o esperado e identificando divergências que afetem a experiência do usuário (UX).

---

## 📋 1. Casos de Teste Executados (Test Cases)

| ID | Módulo | Cenário / Descrição | Pré-condição | Resultado Esperado | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **7220355** | Avaliações e Comentários | Testando interação de like e deslike das avaliações dos produtos | Usuário previamente cadastrado | Conseguir dar like ou deslike nas avaliações dos produtos  | **FAIL** |
| **TC-002** | Autenticação | Tentar login sem preencher o campo de e-mail | Estar na tela de login | Exibir mensagem de alerta: *"Campo obrigatório"* | **PASS** |
| **TC-003** | Interface | Navegação entre guias principais do aplicativo | Usuário logado na conta | Transição fluida de telas sem travamentos ou falhas de layout | **FAIL** |

---

## 🐛 2. Relatório de Defeitos (Bug Report)

Abaixo está o exemplo do padrão de bug report detalhado utilizado durante a execução dos testes:

### [7220355] Falha ao conseguir clicar nos botões de like e deslike

* **Severidade:** Média |
* **Ambiente:** Chrome / Linux Mint

**Passos para Reproduzir:**
1. Vá para [url].
2. Na barra de navegação, clique em qualquer marca.
3. Escolha um produto.
4. Deslize até a aréa de avaliações.
5. Clique no botão de "like" ou "deslike" em qualquer avaliação.

**Resultado Esperado:** 
Usuário deveria dar like ou deslike no comentário avaliando o produto com sucesso.

**Resultado Obtido:** 
O número de likes ou deslikes na avaliação não atualiza.

**Evidências e Logs:**
* Erro registrado no console / captura de tela / video replicando o bug.

---

## 💡 Competências Aplicadas
* Análise de requisitos e instruções do ciclo de testes.
* Execução de testes de regressão e exploratórios.
* Documentação clara e objetiva de defeitos com passos de reprodução.
