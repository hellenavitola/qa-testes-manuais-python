# Casos de Teste — Projeto QA

## TC-001 — Login com campos vazios

**Objetivo:** Verificar o comportamento do sistema ao tentar realizar login sem preencher os campos.

**Pré-condição:** Estar na página Form Authentication do site The Internet.

**Passos executados:**
1. Acessar a página de login.
2. Deixar os campos Username e Password vazios.
3. Clicar no botão Login.

**Resultado esperado:**
O sistema deve impedir o acesso e apresentar uma mensagem adequada informando que os dados são inválidos ou obrigatórios.

**Resultado obtido:**
O sistema exibiu a mensagem: "Your username is invalid".

**Status:** Executado — análise pendente.

**Observação:** É necessário realizar testes adicionais para verificar se a mensagem é consistente com o comportamento esperado.
