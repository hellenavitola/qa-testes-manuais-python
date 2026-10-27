# Relatório de Execução de Testes — Projeto QA

## 1. Sobre o projeto

Projeto de estudo desenvolvido para praticar testes manuais de software utilizando a aplicação de demonstração The Internet, na funcionalidade Form Authentication.

O objetivo é validar o comportamento do login e do encerramento de sessão, documentando os passos executados, os resultados observados e as evidências obtidas.

## 2. Escopo dos testes

Foram realizados testes relacionados a:
- Login com campos vazios.
- Login com usuário inválido.
- Login com senha incorreta.
- Login com credenciais válidas.
- Logout.
- Tentativa de acesso à área segura após o logout.
- Login com senha vazia.
- Login com usuário vazio.
- Navegação de volta após o logout.

## 3. Resumo dos resultados

Os testes realizados apresentaram comportamentos compatíveis com o esperado nos cenários observados.

Durante o teste de navegação após o logout, a área segura reapareceu ao utilizar o botão Voltar do navegador. Após atualizar a página, o sistema exigiu autenticação, indicando que o conteúdo anterior pode ter sido recuperado do cache do navegador.

Não foi confirmada nenhuma falha de segurança durante os testes realizados.

## 4. Conclusão

A execução permitiu praticar a validação de funcionalidades de autenticação, a documentação de casos de teste e a investigação de comportamentos inesperados.

Este projeto está em desenvolvimento e faz parte do meu aprendizado em Qualidade de Software (QA), durante meus estudos em Análise e Desenvolvimento de Sistemas.
