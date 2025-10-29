# Projeto - Modulo 4 (Arquitetura MVC e Padroes de Projeto)

## Desafio: Sistema de Matriculas MVC

### Visao Geral
Implemente um sistema MVC completo para gerenciar matriculas no curso LTP 3, reforcando separacao entre Modelo, Visao e Controle.

### Requisitos Funcionais
1. Cadastro de alunos, modulos e turmas.
2. Matricula e cancelamento com validacao de vagas.
3. Painel administrativo exibindo estatisticas (total de alunos, vagas ocupadas, taxa de conclusao).

### Arquitetura
- **Modelo:** Entidades (`Aluno`, `Turma`, `Matricula`) com regras e invariantes.
- **DAO:** Implementacao JDBC e caches em memoria (Strategy para alternar).
- **Servico:** `MatriculaService` aplicando regras de negocio.
- **Controle:** Servlets mapeados por modulo (`/admin/turmas`, `/admin/alunos`).
- **Visao:** JSPs modulares com JSTL, fragments reutilizaveis e relatorios exportados em CSV.

### Padroes Recomendados
- **DAO:** Abstrair persistencia.
- **Factory Method:** Criar instancias de DAO conforme configuracao (JDBC ou Mock).
- **Front Controller:** Um servlet principal que delega para controladores especificos.
- **Template Method:** Para gerar relatorios com cabecalhos padronizados.

### Entregáveis
- Guia de arquitetura (`docs/arquitetura_mvc.md`) descrevendo diagramas de classes e sequencia.
- Scripts SQL para criacao de tabelas (`database/schema.sql`).
- Testes unitarios para camada de servico com Mockito.
- Scripts de build e deploy (Maven ou Gradle).

---

[Voltar aos Links Rapidos](../README.md#links-rapidos)
