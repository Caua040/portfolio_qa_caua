# 📱 Projeto 1: Suíte de Testes Funcionais & Reporte de Bugs

Este projeto documenta o planejamento, a execução de casos de teste manuais e a identificação de falhas funcionais em aplicações Web/Mobile, com base em cenários práticos e execuções na plataforma **uTest**.

---

## 🎯 Objetivo dos Testes
Validar os fluxos críticos da aplicação (como navegação, cadastro/login, interações da interface e regras de negócio), garantindo que o sistema responda conforme o esperado e identificando divergências que afetem a experiência do usuário (UX).

---

## 📋 1. Casos de Teste Executados (Test Cases)

| ID | Módulo | Cenário / Descrição | Pré-condição | Resultado Esperado | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **TC-001** | Autenticação | Validar login com e-mail e senha válidos | Usuário previamente cadastrado | Redirecionamento para a tela inicial com sucesso | **PASS** |
| **TC-002** | Autenticação | Tentar login sem preencher o campo de e-mail | Estar na tela de login | Exibir mensagem de alerta: *"Campo obrigatório"* | **PASS** |
| **TC-003** | Interface | Navegação entre guias principais do aplicativo | Usuário logado na conta | Transição fluida de telas sem travamentos ou falhas de layout | **FAIL** |

---

## 🐛 2. Relatório de Defeitos (Bug Report)

Abaixo está o exemplo do padrão de bug report detalhado utilizado durante a execução dos testes:

### [BUG-001] Falha de renderização na transição de telas no menu principal

* **Severidade:** Média | **Prioridade:** Média
* **Ambiente:** Android 14 / App v2.4.1 / Conexão Wi-Fi 5G

**Passos para Reproduzir:**
1. Abra o aplicativo e realize o login.
2. No menu inferior, toque rapidamente entre as abas "Início" e "Perfil".
3. Observe o comportamento da interface.

**Resultado Esperado:** 
As telas devem alternar sem sobreposição de elementos ou travamento visual.

**Resultado Obtido:** 
A tela de "Perfil" carrega sobreposta ao conteúdo da aba "Início", congelando a navegação e exigindo o reinício do aplicativo.

**Evidências e Logs:**
* Erro registrado no console / captura de tela de evidência.

---

## 💡 Competências Aplicadas
* Análise de requisitos e instruções do ciclo de testes.
* Execução de testes de regressão e exploratórios.
* Documentação clara e objetiva de defeitos com passos de reprodução.
