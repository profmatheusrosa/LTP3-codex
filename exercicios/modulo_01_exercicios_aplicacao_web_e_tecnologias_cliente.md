# Exercicios - Modulo 1 (Aplicacao Web e Tecnologias do Lado Cliente)

## Exercicios Propostos

### Exercicio 1 - Mapeando Fluxo Cliente-Servidor
Implemente um diagrama em Mermaid ou desenhe a mao (digitalizando) representando o fluxo completo de uma requisicao HTTP entre cliente e servidor, destacando:
- Navegador enviando requisicao GET para `/cursos`.
- Servidor roteando a requisicao para um controlador.
- Controlador consultando uma camada de servico.
- Servico acessando um DAO para buscar dados em memoria.
- DAO retornando lista de cursos para o controlador.
- Controlador encaminhando a resposta para uma JSP.

Entregue:
1. Arquivo `diagramas/fluxo_cliente_servidor.mmd` com o diagrama em Mermaid.
2. Resumo em Markdown explicando cada etapa e mencionando cabecalhos HTTP importantes (`Accept`, `Content-Type`, `Cache-Control`).

### Exercicio 2 - Landing Page XHTML + CSS
Construa uma landing page estatica para apresentar o curso LTP 3:
1. Utilize XHTML bem formado (declare `<?xml version="1.0" encoding="UTF-8"?>` e `<!DOCTYPE html>`).
2. A pagina deve conter `header`, `nav`, `main`, `section` e `footer`.
3. Crie um arquivo CSS externo (`public/css/landing.css`) usando Flexbox para alinhar cards de modulos.
4. Inclua um formulario de inscricao que envie dados via `POST` para `/inscricoes`.
5. Garanta compatibilidade mobile (layout responsivo com `@media`).

Entregue a pagina em `public/index.xhtml` e aplique classes e IDs descritivos.

### Exercicio 3 - Formulario Dinamico com JavaScript
Adicione interatividade ao formulario da landing page:
1. Crie o arquivo `public/js/formulario.js`.
2. Valide campos obrigatorios (nome, email, modulo de interesse) antes do envio com mensagens exibidas no DOM.
3. Use `fetch` para enviar a inscricao para `/api/inscricoes` exibindo uma notificacao de sucesso ou erro sem recarregar a pagina.
4. Simule a resposta do servidor com `setTimeout` caso o endpoint real nao esteja disponivel.

Documente as decisoes em `docs/notas_modulo_01.md` incluindo passos de configuracao e navegadores testados.

---

[Voltar aos Links Rapidos](../README.md#links-rapidos)
