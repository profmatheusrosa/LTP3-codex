# Projeto - Modulo 5 (Projeto de Conclusao)

## Desafio Final: Sistema Integrado de Gestao de Cursos

### Objetivo
Entregar uma aplicacao completa integrando todas as camadas abordadas ao longo do curso, pronta para deploy em servidor Java.

### Escopo Funcional
1. **Gestao de Usuarios**
   - Cadastro, autenticacao e autorizacao (perfis: admin, instrutor, aluno).
   - Recuperacao de senha via email (mock).
2. **Catálogo de Cursos**
   - CRUD de cursos, modulos e aulas.
   - Agenda de turmas com controle de vagas.
3. **Matriz de Aprendizado**
   - Liberacao de conteudos conforme progresso.
   - Feedback de avaliacao (formulario + relatorios).

### Arquitetura Exigida
- Front Controller servlet para roteamento central.
- JSPs com JSTL/EL como camada de visao.
- Servicos aplicando regras de negocio.
- DAOs com implementacao JPA/Hibernate e fallback em memoria.
- Camada de integracao com API externa (mock) para notificacoes.

### Requisitos Não Funcionais
- Testes de unidade (JUnit 5 + Mockito) e integracao (Testcontainers).
- Logs estruturados com SLF4J + Logback.
- Pipeline CI/CD automatizado (GitHub Actions).
- Guia de deploy em servidor Tomcat e em container Docker.

### Entregáveis
- Codigo fonte completo.
- Documentacao `docs/manual_deploy.md` detalhando configuracao, scripts SQL e variaveis de ambiente.
- Colecao de requisicoes REST (Insomnia/Postman) para validacao manual.
- Apresentacao (slides ou video) resumindo arquitetura, desafios e proximos passos.

---

[Voltar aos Links Rapidos](../README.md#links-rapidos)
