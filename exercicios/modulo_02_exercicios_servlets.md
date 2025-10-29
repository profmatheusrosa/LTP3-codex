# Exercicios - Modulo 2 (Servlets)

## Exercicios Propostos

### Exercicio 1 - Servlet de Cadastro
Implemente um servlet `CadastroCursoServlet` que:
1. Responda a `POST /cursos` recebendo dados (`nome`, `cargaHoraria`, `descricao`).
2. Valide campos obrigatorios, retornando `400 Bad Request` com mensagem JSON quando houver erro.
3. Armazene os cursos em uma lista em memoria (usar `ServletContext` para compartilhar estado).
4. Retorne `201 Created` com corpo JSON contendo o identificador gerado.

Crie testes de integracao com `HttpUnit` ou `MockMvc` (Spring Test) para validar os cenarios de sucesso e erro.

### Exercicio 2 - Servlet de Listagem com Filtro
Crie o servlet `ListarCursosServlet` que:
1. Atenda `GET /cursos` devolvendo HTML renderizado em JSP.
2. Aceite parametro `categoria` e filtre a lista.
3. Defina atributos `cursos` (lista filtrada) e `categoriasDisponiveis` para a JSP `cursos.jsp`.
4. Utilize `RequestDispatcher` para encaminhar a requisicao.

Documente em `docs/modulo_02_servlets.md` endpoints, parametros, exemplos de resposta e consideracoes sobre thread safety.

---

[Voltar aos Links Rapidos](../README.md#links-rapidos)
