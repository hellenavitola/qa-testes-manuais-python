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

Foram executados nove casos de teste manuais relacionados à autenticação e ao encerramento de sessão.

Nos testes de login com credenciais inválidas ou campos vazios, o sistema impediu o acesso e apresentou mensagens de erro compatíveis com as situações observadas. Com credenciais válidas, o acesso à área segura foi permitido.

O logout retornou à página de login. Durante o teste de navegação pelo botão Voltar, a área segura reapareceu no navegador, mas, após atualizar a página, o sistema exigiu autenticação novamente.

Esse comportamento foi registrado para investigação, considerando a possibilidade de exibição de conteúdo armazenado em cache. Não foi confirmada uma falha de segurança.

Os resultados representam as observações realizadas durante os testes manuais e não constituem uma certificação completa da segurança da aplicação.

## 4. Conclusão

A execução permitiu praticar a validação de funcionalidades de autenticação, a documentação de casos de teste e a investigação de comportamentos inesperados.

Este projeto está em desenvolvimento e faz parte do meu aprendizado em Qualidade de Software (QA), durante meus estudos em Análise e Desenvolvimento de Sistemas.
