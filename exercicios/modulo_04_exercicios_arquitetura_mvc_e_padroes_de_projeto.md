# Exercicios - Modulo 4 (Arquitetura MVC e Padroes de Projeto)

## Exercicios Propostos

### Exercicio 1 - Refatoracao para MVC
Receba um projeto legado onde uma unica JSP contem logica de negocio e acesso a banco. Refatore para arquitetura MVC:
1. Crie entidades `Curso`, `Modulo`, `Instrutor`.
2. Implemente DAOs (`CursoDao`, `ModuloDao`) para acesso a dados.
3. Construa servico `CatalogoService` que orquestra regras (validacao de carga horaria, publicacao).
4. Defina controlador (`CatalogoController`) que popula atributos e encaminha para JSP.
5. Documente mudancas em `docs/refatoracao_mvc.md` descrevendo ganhos de coesao e testabilidade.

### Exercicio 2 - DAO com Testes
1. Implemente `CursoDaoJdbc` com operacoes CRUD usando `PreparedStatement`.
2. Utilize banco em memoria H2 para testes.
3. Crie testes com `@BeforeEach` inserindo dados basicos.
4. Garanta fechamento de recursos (`try-with-resources`) e trate excecoes transformando-as em `RuntimeException` customizada.
5. Escreva README curto em `docs/dao_h2.md` explicando configuracoes e estrategia de transacao.

---

[Voltar aos Links Rapidos](../README.md#links-rapidos)
