# Resultados dos Testes — Projeto QA

## Resumo da execução

| ID | Cenário de teste | Resultado observado |
|---|---|---|
| TC-001 | Login com campos vazios | Sistema informou que o usuário era inválido |
| TC-002 | Login com usuário inválido | Sistema rejeitou o usuário |
| TC-003 | Login com senha incorreta | Sistema rejeitou a senha |
| TC-004 | Login com credenciais válidas | Login realizado com sucesso |
| TC-005 | Logout | Retorno à página de login |
| TC-006 | Acesso à área segura após logout | Sistema solicitou autenticação |
| TC-007 | Login com senha vazia | Sistema rejeitou a senha |
| TC-008 | Login com usuário vazio | Sistema rejeitou o usuário |
| TC-009 | Botão Voltar após logout | Área segura reapareceu; após atualizar, o sistema exigiu autenticação |

## Observações

Os testes foram executados manualmente no site de demonstração The Internet.

O comportamento observado no TC-009 foi investigado com uma atualização da página. Não foi confirmada uma falha de segurança.

Este relatório registra os resultados observados durante a execução dos testes e faz parte de um projeto de aprendizagem em QA.
