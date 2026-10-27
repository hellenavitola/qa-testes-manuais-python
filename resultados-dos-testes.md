# Resultados dos Testes — Projeto QA

## 1. Resumo da execução

Foram executados nove casos de teste manuais na funcionalidade Form Authentication do site The Internet.

| ID | Cenário | Resultado observado | Avaliação |
|---|---|---|---|
| TC-001 | Login com campos vazios | Mensagem de usuário inválido | Compatível com o esperado |
| TC-002 | Usuário inválido | Mensagem de usuário inválido | Compatível com o esperado |
| TC-003 | Senha incorreta | Mensagem de senha inválida | Compatível com o esperado |
| TC-004 | Credenciais válidas | Acesso permitido e mensagem de sucesso | Compatível com o esperado |
| TC-005 | Logout | Retorno à tela de login | Compatível com o esperado |
| TC-006 | Acesso à área segura após logout | Sistema solicitou autenticação | Compatível com o esperado |
| TC-007 | Senha vazia | Mensagem de senha inválida | Compatível com o esperado |
| TC-008 | Usuário vazio | Mensagem de usuário inválido | Compatível com o esperado |
| TC-009 | Botão Voltar após logout | Área segura reapareceu; após atualizar, o sistema exigiu autenticação | Investigação realizada; nenhuma falha confirmada |

## 2. Observações

Os testes foram realizados manualmente e os resultados foram registrados conforme o comportamento observado na aplicação.

No TC-009, a área segura reapareceu após o uso do botão Voltar do navegador. Ao atualizar a página, o sistema exigiu autenticação. O comportamento pode estar relacionado ao cache do navegador, mas essa hipótese não foi confirmada tecnicamente.

## 3. Conclusão

Os testes permitiram praticar a validação de funcionalidades de autenticação, a documentação de resultados e a investigação de comportamentos inesperados.

Este projeto é uma iniciativa de aprendizagem em Qualidade de Software (QA), desenvolvida durante os estudos em Análise e Desenvolvimento de Sistemas. Os resultados estão limitados aos cenários executados e não representam uma avaliação completa da aplicação.
