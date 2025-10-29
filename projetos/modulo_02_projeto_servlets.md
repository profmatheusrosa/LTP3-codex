# Projeto - Modulo 2 (Servlets)

## Desafio: API de Gerenciamento de Turmas

### Cenário
Construa uma API baseada em servlets para gerir turmas do curso LTP 3. A aplicacao deve fornecer operações CRUD e garantir consistencia dos dados.

### Escopo
1. **Modelos**
   - `Turma` (id, modulo, instrutor, capacidade, dataInicio, dataFim).
   - `Aluno` (id, nome, email, status).

2. **Endpoints**
   - `POST /turmas` cria turma.
   - `GET /turmas` lista turmas com filtros (`modulo`, `status`).
   - `POST /turmas/{id}/matriculas` matricula aluno.
   - `DELETE /turmas/{id}/matriculas/{alunoId}` cancela matricula.

3. **Tecnologia**
   - Servlets puros (sem frameworks) com `HttpServlet`.
   - Serializacao JSON utilizando `Jackson` ou `Gson`.
   - Persistencia temporaria em memoria (Collections sincronizadas).

### Requisitos
- Implementar camada de servico isolada para regras (capacidade da turma, status de matricula).
- Aplicar filtros via query string (`/turmas?modulo=3`).
- Configurar `ServletContextListener` para carregar dados iniciais.
- Fornecer documentacao (`docs/api_turmas.md`) com exemplos de requisicao/resposta.
- Incluir testes de integracao com `JUnit` e `MockHttpServletRequest/Response`.

### Critérios de Avaliação
- Uso correto do ciclo de vida de servlets.
- Tratamento de erros com codigos HTTP apropriados.
- Codigo organizado e thread-safe.
- Documentacao clara e reutilizavel.

---

[Voltar aos Links Rapidos](../README.md#links-rapidos)
