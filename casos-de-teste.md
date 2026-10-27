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
## TC-002 — Login com usuário inválido

**Objetivo:** Verificar se o sistema impede o acesso quando o nome de usuário informado não existe ou é inválido.

**Pré-condição:** Estar na página Form Authentication do site The Internet.

**Passos executados:**
1. Preencher Username com `usuario_teste_123`.
2. Preencher Password com `senha_incorreta_123`.
3. Clicar no botão Login.

**Resultado esperado:**
O sistema deve impedir o acesso e informar que as credenciais são inválidas.

**Resultado obtido:**
O sistema exibiu a mensagem: "Your username is invalid".

**Status:** Executado — comportamento observado compatível com o esperado.

**Observação:** Este teste não permite avaliar isoladamente a validação da senha, pois o nome de usuário informado também é inválido.
## TC-003 — Login com senha incorreta

**Objetivo:** Verificar se o sistema impede o acesso quando o usuário é válido, mas a senha está incorreta.

**Pré-condição:** Estar na página Form Authentication do site The Internet.

**Passos executados:**
1. Preencher Username com `tomsmith`.
2. Preencher Password com `senha_incorreta_123`.
3. Clicar no botão Login.

**Resultado esperado:**
O sistema deve impedir o acesso e informar que a senha é inválida.

**Resultado obtido:**
O sistema exibiu a mensagem: "Your password is invalid".

**Status:** Executado — comportamento observado compatível com o esperado.

**Observação:** O sistema diferenciou a mensagem de usuário inválido da mensagem de senha inválida, conforme observado nos testes anteriores.
## TC-004 — Login com credenciais válidas

**Objetivo:** Verificar se o sistema permite o acesso quando o usuário e a senha estão corretos.

**Pré-condição:** Estar na página Form Authentication do site The Internet.

**Passos executados:**
1. Preencher Username com `tomsmith`.
2. Preencher Password com `SuperSecretPassword!`.
3. Clicar no botão Login.

**Resultado esperado:**
O sistema deve permitir o acesso e exibir uma mensagem de sucesso, além de disponibilizar a opção de sair da área autenticada.

**Resultado obtido:**
O sistema exibiu a mensagem de sucesso e o botão Logout.

**Status:** Executado — comportamento observado compatível com o esperado.

**Observação:** As credenciais válidas permitiram o acesso à área autenticada.
## TC-005 — Logout (encerrar sessão)

**Objetivo:** Verificar se o sistema permite encerrar a sessão após um login bem-sucedido.

**Pré-condição:** Estar autenticada na área segura do site The Internet.

**Passos executados:**
1. Realizar login com credenciais válidas.
2. Clicar no botão Logout.
3. Observar a página exibida após a saída.

**Resultado esperado:**
O sistema deve encerrar a sessão e retornar à página de login.

**Resultado obtido:**
O sistema retornou à página de login sem exibir mensagem de sucesso.

**Status:** Executado — comportamento observado compatível com o esperado.

**Observação:** O retorno à página de login foi confirmado. Este teste não verificou, isoladamente, se o acesso à área segura permanece bloqueado após o logout.
## TC-006 — Acessar área segura após logout

**Objetivo:** Verificar se o sistema impede o acesso à área segura após o encerramento da sessão.

**Pré-condição:** Ter realizado login com credenciais válidas e encerrado a sessão por meio do botão Logout.

**Passos executados:**
1. Realizar logout.
2. Digitar `https://the-internet.herokuapp.com/secure` diretamente na barra de endereço do navegador.
3. Pressionar Enter.
4. Observar o comportamento do sistema.

**Resultado esperado:**
O sistema deve impedir o acesso à área segura sem autenticação e redirecionar o usuário para a página de login ou solicitar que ele entre novamente.

**Resultado obtido:**
O sistema redirecionou para a página de login ou solicitou autenticação.

**Status:** Executado — comportamento observado compatível com o esperado.

**Observação:** O acesso à área segura foi bloqueado após o logout, conforme o comportamento observado.
## TC-007 — Login com senha vazia

**Objetivo:** Verificar se o sistema impede o login quando o usuário é válido, mas o campo de senha não é preenchido.

**Pré-condição:** Estar na página Form Authentication do site The Internet.

**Passos executados:**
1. Preencher Username com `tomsmith`.
2. Deixar o campo Password vazio.
3. Clicar no botão Login.

**Resultado esperado:**
O sistema deve impedir o acesso e informar que a senha é inválida ou que o preenchimento da senha é obrigatório.

**Resultado obtido:**
O sistema exibiu a mensagem: "Your password is invalid".

**Status:** Executado — comportamento observado compatível com o esperado.

**Observação:** O usuário foi aceito, mas o sistema rejeitou a tentativa de login sem uma senha válida.
## TC-008 — Login com usuário vazio

**Objetivo:** Verificar se o sistema impede o login quando o campo de usuário está vazio, mesmo que a senha seja preenchida.

**Pré-condição:** Estar na página Form Authentication do site The Internet.

**Passos executados:**
1. Deixar o campo Username vazio.
2. Preencher Password com `SuperSecretPassword!`.
3. Clicar no botão Login.

**Resultado esperado:**
O sistema deve impedir o acesso e informar que o usuário é inválido ou que o preenchimento do campo é obrigatório.

**Resultado obtido:**
O sistema exibiu a mensagem: "Your username is invalid".

**Status:** Executado — comportamento observado compatível com o esperado.

**Observação:** O sistema rejeitou a tentativa de login com o campo Username vazio, apesar de a senha ter sido preenchida.
