# Projeto - Modulo 3 (Java Server Pages)

## Desafio: Portal Administrativo JSP

### Objetivo
Construir um portal administrativo que permita gerenciar conteudos do curso utilizando JSP, JSTL e EL, mantendo separacao clara entre camada de apresentacao e regras.

### Funcionalidades
1. **Autenticacao Simples**
   - Tela de login (`login.jsp`) com feedback de erros via EL.
   - Verificacao de credenciais em servlet dedicado (`LoginServlet`).

2. **Gestao de Conteudos**
   - Listagem de aulas (`aulas.jsp`) com tabela responsiva.
   - Formulario de cadastro/edicao com `jsp:include` para reaproveitar campos.
   - Paginacao controlada por parametros (`pagina`, `limite`).

3. **Feedback e Internacionalizacao**
   - Mensagens armazenadas em `ResourceBundle` e acessadas via `<fmt:message>`.
   - Layout base reutilizavel com `jsp:include` e fragmentos.

### Requisitos Técnicos
- Estrutura sugerida:
  ```
  portal-admin/
  ├── src/main/java/
  │   └── br/com/ltp3/web
  ├── src/main/webapp/
  │   ├── WEB-INF/views/
  │   │   ├── layout/
  │   │   │   └── base.jsp
  │   │   ├── login.jsp
  │   │   └── aulas.jsp
  │   └── WEB-INF/lib/
  └── src/main/resources/messages.properties
  ```
- Proibir scriptlets; utilizar apenas JSTL/EL.
- Criar filtros (`Filter`) para proteger rotas autenticadas.
- Registrar tags personalizadas se necessario (ex: tag para badges de status).

### Entregáveis
- Codigo fonte completo com instrucoes de build (Maven/Gradle).
- Guia `docs/portal_admin_manual.md` explicando arquitetura, navegacao e configuracao.
- Capturas de tela demonstrando recursos principais.

---

[Voltar aos Links Rapidos](../README.md#links-rapidos)
