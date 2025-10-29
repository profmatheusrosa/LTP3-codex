# Exercicios - Modulo 3 (Java Server Pages)

## Exercicios Propostos

### Exercicio 1 - Dashboard com JSTL
1. Crie a JSP `WEB-INF/views/dashboard.jsp`.
2. Utilize JSTL `c:forEach` para listar os modulos do curso, exibindo progresso e instrutor.
3. Quando a lista estiver vazia, apresente mensagem usando `c:if`.
4. Formate datas com `<fmt:formatDate>` (locale `pt_BR`).
5. Substitua qualquer scriptlet existente por EL e JSTL.

Defina o controlador correspondente e envie os atributos `modulos` e `ultimaAtualizacao` via servlet.

### Exercicio 2 - Formulario com Validação EL
1. Implemente a JSP `WEB-INF/views/inscricao.jsp`.
2. Utilize EL para exibir mensagens de validacao vindas de `requestScope.erros`.
3. Preencha campos com valores anteriores usando `${param.nome}`.
4. Use `<c:choose>` para exibir variacoes de layout conforme o modulo selecionado.

Documente boas praticas em `docs/modulo_03_jsp.md`, citando como evitar scriptlets e riscos de concorrencia.

---

[Voltar aos Links Rapidos](../README.md#links-rapidos)
