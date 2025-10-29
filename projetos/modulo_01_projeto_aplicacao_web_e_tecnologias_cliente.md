# Projeto - Modulo 1 (Aplicacao Web e Tecnologias do Lado Cliente)

## Desafio: Portal de Conteudos Educacionais

### Cenário
Uma escola tecnica deseja publicar conteudos de cursos no formato web. O portal deve exibir lista de cursos, permitir busca por palavra-chave e coletar inscricoes iniciais de interessados.

### Objetivos
1. **Frontend XHTML/CSS**
   - Estruture a pagina inicial em XHTML semantico.
   - Utilize CSS Grid para exibir cards de cursos responsivos.
   - Inclua breadcrumb e navegação destacando seções “Cursos”, “Instrutores” e “Planos”.

2. **Interacao JavaScript**
   - Implementar busca com filtro em tempo real utilizando JavaScript.
   - Apresentar modal com detalhes do curso quando o usuario clicar em um card.
   - Registrar o interesse (POST em `/api/interesse`) com feedback visual.

3. **Acessibilidade e Performance**
   - Aplicar atributos `aria-*`, contraste adequado e suporte a teclado.
   - Otimizar assets (minificacao e lazy loading de imagens).

### Requisitos Tecnicos
- Configurar estrutura de pastas:
  ```
  portal/
  ├── public/
  │   ├── index.xhtml
  │   ├── cursos.xhtml
  │   ├── css/
  │   │   └── estilos.css
  │   └── js/
  │       └── portal.js
  └── docs/
      └── guia_estilo.md
  ```
- Documentar no `docs/guia_estilo.md` paleta de cores, tipografia e componentes reutilizaveis.
- Entregar script `public/js/portal.js` comentado com as funcoes principais.

### Critérios de Avaliação
- Layout responsivo e semanticamente correto.
- Codigo JavaScript modular, reutilizavel e com tratamento de erros.
- Documentacao clara e aderente ao estilo corporativo.
- Demonstração (screencast curto ou PDF com capturas) destacando funcionalidades.

---

[Voltar aos Links Rapidos](../README.md#links-rapidos)
