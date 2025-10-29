## Objetivo
Criar um repositório Git completo para um novo curso, seguindo uma estrutura padronizada e incluindo módulos teóricos detalhados, exercícios de fixação, projetos práticos e materiais complementares. O repositório final deve ser compactado em um arquivo ZIP.

## Entrada Necessária

### 1. Nome do Curso
LTP 3

### 2. Carga Horária Total do Curso (em horas)
80h

### 3. Carga Horária Sugerida por Aula
2h

### 4. Conteúdo do Curso
| **Módulo**   | **Tópicos Principais**                       | **Subtópicos**                                                                                   | **Detalhes**                                                                 |
|--------------|----------------------------------------------|--------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------|
| **Módulo 1** | 1. Aplicação Web                             | 1.1 Arquitetura e Funcionamento                                                                  | Conceito geral, interação cliente-servidor                                   |
|              |                                              | 1.2 Cliente Web                                                                                  | Navegadores, funções básicas                                                 |
|              |                                              | 1.3 Servidor Web                                                                                 | Funções, exemplos, hospedagem                                                |
|              |                                              | 1.4 Protocolo HTTP                                                                               | Métodos, cabeçalhos, requisição e resposta                                   |
|              | 2. Tecnologias do Lado Cliente               | 2.1 Marcação XHTML                                                                                | Estrutura, sintaxe, boas práticas                                            |
|              |                                              | 2.2 Estilos CSS                                                                                  | Seletores, propriedades, layout                                              |
|              |                                              | 2.3 Scripts JavaScript                                                                           | Manipulação de DOM, eventos, validações                                     |
| **Módulo 2** | 3. Servlets                                   | 3.1 Definição                                                                                     | Conceito e finalidade                                                         |
|              |                                              | 3.2 Ciclo de Vida                                                                                 | init, service, destroy                                                        |
|              |                                              | 3.3 Tratamento de Solicitações GET e POST                                                         | Diferenças e usos                                                             |
|              |                                              | 3.4 Parâmetros e Respostas                                                                       | Obtenção de parâmetros, envio de respostas                                  |
|              |                                              | 3.5 Redirecionamento e Encaminhamento                                                            | sendRedirect, forward                                                         |
|              |                                              | 3.6 Seções                                                                                        | Criação, uso, gerenciamento de sessão                                        |
| **Módulo 3** | 4. Java Server Pages (JSP) – Parte 1          | 4.1 Scriptlets                                                                                    | Código Java embutido                                                          |
|              |                                              | 4.2 Declarações                                                                                   | Definição de variáveis e métodos                                              |
|              |                                              | 4.3 Expressões                                                                                    | Exibição de valores                                                           |
|              |                                              | 4.4 Objetos Implícitos                                                                            | request, response, session, application                                      |
|              | 5. Java Server Pages (JSP) – Parte 2          | 5.1 Diretivas                                                                                     | page, include, taglib                                                          |
|              |                                              | 5.2 Ações                                                                                         | `<jsp:useBean>`, `<jsp:setProperty>`, etc.                                    |
|              |                                              | 5.3 Linguagem de Expressão – EL                                                                   | Sintaxe, operadores, integração com JSP                                      |
|              |                                              | 5.4 Biblioteca de Tags Padrão – JSTL                                                              | Core, format, SQL, funções                                                    |
| **Módulo 4** | 6. Arquitetura MVC e Padrões de Projeto       | 6.1 Visão Geral                                                                                   | Conceito, benefícios                                                          |
|              |                                              | 6.2 Camada Modelo                                                                                 | Classes Java, entidades, regras de negócio                                   |
|              |                                              | 6.3 Camada de Acesso a Dados (DAO)                                                                | Padrão DAO, CRUD                                                              |
|              |                                              | 6.4 Camada Visão                                                                                  | JSP para exibição de dados                                                    |
|              |                                              | 6.5 Camada Controle                                                                               | Servlets controlando fluxo e lógica                                          |
| **Módulo 5** | 7. Projeto de Conclusão de Curso              | 7.1 Desenvolvimento                                                                               | Integração de todos os conceitos: MVC, DAO, JSP, Servlets, Cliente e Servidor |

## Estrutura do Repositório (Exemplo: curso_novo_nome/)

```
curso_novo_nome/
├── teoria/
│   ├── modulo_01_titulo_do_modulo.md
│   ├── modulo_02_titulo_do_modulo.md
│   └── ...
├── exercicios/
│   ├── modulo_01_exercicios_titulo_do_modulo.md
│   ├── modulo_02_exercicios_titulo_do_modulo.md
│   └── ...
├── projetos/
│   ├── modulo_01_projeto_titulo_do_modulo.md
│   ├── modulo_02_projeto_titulo_do_modulo.md
│   └── ...
├── materiais_complementares/
│   ├── glossario_novo_nome.md
│   ├── cheatsheet_novo_nome.md
│   ├── roadmap_carreira_novo_nome.md
│   └── ferramentas_e_softwares_novo_nome.md
├── imagens/
│   ├── imagem_conceito_1.png
│   ├── imagem_conceito_2.png
│   └── ...
├── README.md
├── planejamento_aulas.md
└── LICENSE
```

## Passos Detalhados para a Criação

### 1. Configuração Inicial

- Criar o diretório principal do curso (ex: curso_novo_nome).
- Dentro do diretório principal, criar os subdiretórios: teoria, exercicios, projetos, materiais_complementares, imagens.

### 2. Criação dos Módulos Teóricos (teoria/)

- Para cada tópico principal fornecido, criar um arquivo Markdown com um nome significativo (ex: modulo_XX_titulo_do_modulo.md). O titulo_do_modulo deve ser uma versão "slugified" do título do módulo (minúsculas, espaços por underscores, sem caracteres especiais).

- **Conteúdo de cada arquivo teórico:**

  - **Título do Módulo.**
  
  - **Sumário Navegável:** Uma lista de links para as seções (##) e subseções (###) dentro do próprio documento. O sumário deve ser gerado automaticamente com base nos títulos das seções.
  
  - **Introdução ao Módulo:** Um parágrafo conciso descrevendo o que será abordado.
  
  - **Conteúdo Teórico Detalhado:** Explicação aprofundada de cada conceito do tópico, com exemplos de código quando aplicável.
  
  - **Imagens Ilustrativas:** Sempre que possível, gerar e incluir imagens relevantes para ilustrar os conceitos. As imagens devem ser salvas na pasta `imagens/` e referenciadas no Markdown (ex: `![Descrição da Imagem](../../imagens/nome_da_imagem.png)`). O nome da imagem deve ser significativo e descritivo.
  - **Caso não seja possível gerar as imagens:**
    - Criar um arquivo `lista_imagens_a_gerar.md` dentro da pasta `imagens/`.
    - Neste arquivo, listar detalhadamente cada imagem que precisa ser criada, incluindo:
      - **Módulo:** O módulo teórico onde a imagem será inserida.
      - **Placeholder:** O texto do placeholder usado no arquivo `.md` (ex: `[IMAGEM_CONCEITO_EVENT_LOOP]`).
      - **Descrição:** Uma descrição clara do que a imagem deve conter.
      - **Prompt de Criação:** O prompt em inglês exato que pode ser usado para gerar a imagem.
    - Nos arquivos de teoria (`.md`), inserir placeholders onde as imagens deveriam estar (ex: `[IMAGEM_CONCEITO_EVENT_LOOP]`).
  
  - **Exercícios de Fixação (Múltipla Escolha):** Ao final de cada seção ou subseção importante, incluir 1-2 questões de múltipla escolha com 4 opções e a resposta correta indicada. As respostas devem ser ocultadas usando as tags `<details>` e `<summary>` do Markdown. **A numeração deve seguir o padrão do módulo: Módulo 1 = Ex 1, 1.1; Módulo 2 = Ex 2, 2.1; etc.** O formato deve ser:

    ```
    **Exercício 1:** [Pergunta da questão]
    a) [Opção A]

    b) [Opção B]

    c) [Opção C]

    d) [Opção D]

    <details>
    <summary>Ver Resposta</summary>
    
    **Resposta:** [Letra da Resposta Correta]) [Opção Correta]
    
    **Explicação:** [Comentário explicativo detalhado sobre por que essa é a resposta correta, conceitos relacionados e informações complementares para aprofundar o conhecimento]
    </details>


    **Exercício 1.1:** [Pergunta da questão]
    a) [Opção A]

    b) [Opção B]

    c) [Opção C]
    
    d) [Opção D]

    <details>
    <summary>Ver Resposta</summary>
    
    **Resposta:** [Letra da Resposta Correta]) [Opção Correta]
    
    **Explicação:** [Comentário explicativo detalhado sobre por que essa é a resposta correta, conceitos relacionados e informações complementares para aprofundar o conhecimento]
    </details>
    ```

  - **Links de Navegação ao Final:** Ao término de cada arquivo de teoria, incluir:
    - Link "Próximo módulo" apontando para o arquivo do próximo módulo (quando houver), usando caminho relativo, por exemplo: `[Próximo módulo →](../teoria/modulo_02_titulo_do_modulo.md)`.
    - Link "Voltar aos Links Rápidos" apontando diretamente para a seção de links rápidos no `README.md`, por exemplo: `[Voltar aos Links Rápidos](../README.md#links-rapidos)` ou `../../README.md#links-rapidos`, ajustando conforme a profundidade do arquivo.
    - Verificar que os caminhos relativos estejam corretos conforme a estrutura adotada.

### 3. Criação dos Exercícios Práticos (exercicios/)

- Para cada módulo teórico, criar um arquivo Markdown com um nome significativo (ex: modulo_XX_exercicios_titulo_do_modulo.md).
- **Conteúdo de cada arquivo de exercícios:**
  - Título do Módulo de Exercícios.
  - Descrição de 1-2 exercícios práticos que complementem a teoria do módulo. Os exercícios devem ser mais elaborados que os de múltipla escolha, exigindo codificação.
  - Incluir exemplos de código ou trechos de código para auxiliar, se necessário.
- Ao final do arquivo, inserir um separador (`---`) seguido do link `[Voltar aos Links Rápidos](../README.md#links-rapidos)` para facilitar a navegação (ajuste o caminho relativo conforme necessário).

### 4. Criação dos Projetos Práticos (projetos/)

- Para cada módulo teórico, criar um arquivo Markdown com um nome significativo (ex: modulo_XX_projeto_titulo_do_modulo.md).
- **Conteúdo de cada arquivo de projeto:**
  - Título do Projeto do Módulo.
  - Descrição de um projeto prático que integre os conceitos aprendidos no módulo e, se possível, nos módulos anteriores.
  - Fornecer um cenário, requisitos e possíveis etapas de implementação.
  - Se o projeto exigir dados, criar arquivos de dados simulados na raiz do repositório (ex: dados_projeto_X.csv) e referenciá-los. O nome do arquivo de dados deve ser significativo.
- Encerrar o documento com um separador (`---`) e o link `[Voltar aos Links Rápidos](../README.md#links-rapidos)` (ajustando o caminho relativo) para manter a navegação consistente.

### 5. Criação dos Materiais Complementares (materiais_complementares/)

- **Glossário:** Criar glossario_novo_nome.md com termos técnicos relevantes para o curso e suas definições.
- **Cheatsheet:** Criar cheatsheet_novo_nome.md com um resumo rápido de sintaxe, comandos ou conceitos chave (ex: cheatsheet_java_swing_jdbc.md).
- **Roadmap de Carreira:** Criar roadmap_carreira_novo_nome.md com sugestões de trilhas de carreira ou próximos passos após o curso.
- **Ferramentas e Softwares:** Criar ferramentas_e_softwares_novo_nome.md com uma lista de ferramentas, IDEs e softwares recomendados.

### 6. Finalização do Repositório

**README.md (template e regras obrigatórias)**

O `README.md` deve existir na raiz do repositório e seguir um template padronizado. Abaixo está o template mínimo recomendado (inclua exatamente essas seções e mantenha links relativos):

1) Cabeçalho e visão geral

- Título do curso (H1)
- Breve descrição do que o curso cobre (1-3 linhas)
- Metadados (Carga horária total, carga horária por aula)

2) Estrutura de Pastas

- Exiba um diagrama simples da estrutura do repositório (texto) com os principais diretórios: `teoria/`, `exercicios/`, `projetos/`, `materiais_complementares/`, `imagens/`, `planejamento_aulas.md`, `LICENSE`

3) Conteúdo Programático (tabela)

- Uma tabela resumida com colunas: `Módulo` | `Tópicos Principais` | `Subtópicos` | `Detalhes`.
- Cada módulo deve aparecer com o título formal: `Módulo X: Nome do Módulo`.

4) Links Rápidos (obrigatório e padronizado)

- Substitua a lista longa por uma tabela compacta com 4 colunas: `Módulo` | `Teoria` | `Exercícios` | `Projeto`.
- Cada célula de link deve apontar para o arquivo relativo correto. Exemplo de linha:

  | Módulo 1<br>Introdução ao Node.js | [Teoria](teoria/modulo_01_introducao_ao_nodejs.md) | [Exercícios](exercicios/modulo_01_exercicios_introducao_ao_nodejs.md) | [Projeto](projetos/modulo_01_projeto_introducao_ao_nodejs.md) |

- Regras para Links Rápidos:
  - Use caminhos relativos (sem links absolutos nem URLs externas) para referência local.
  - Se um tipo de recurso não existir (por exemplo, projeto não criado), mantenha a célula vazia ou escreva `—` para indicar inexistência.
  - Não duplique linhas; uma linha por módulo.

5) Planejamento das Aulas

- Inclua um link para `planejamento_aulas.md` e um resumo breve da distribuição de aulas/módulos.
- Não adicionar seções extras de instruções operacionais ou checklists no README; a navegação deve ser conduzida pelos Links Rápidos e pelos links de retorno presentes nos arquivos de teoria, exercícios e projetos.

6) Pré-requisitos e Ambiente de Desenvolvimento

- Liste configurações mínimas recomendadas.

7) Integridade Acadêmica

- Inclua uma política clara incentivando esforço próprio, uso responsável de ferramentas (incluindo IA) e repúdio a cópias.
- Recomenda-se um texto motivacional enfatizando que exercícios e projetos são oportunidades reais de aprendizagem e construção de caráter.

8) Exemplo de Template de README (markdown)

Inclua no arquivo de orientações um exemplo completo mínimo do `README.md` (substitua textos por placeholders):

```markdown
# Curso de Exemplo: Nome do Curso

Breve descrição do curso...

## Visão Geral do Curso

- **Carga Horária Total:** 60 horas
- **Duração por Aula:** 1 hora

## Estrutura de Pastas

```
curso_novo_nome/
├── teoria/
├── exercicios/
├── projetos/
├── materiais_complementares/
├── imagens/
├── README.md
├── planejamento_aulas.md
└── LICENSE
```

## Conteúdo Programático

| Módulo | Tópicos Principais | Subtópicos | Detalhes |
|--------|-------------------|------------|----------|
| Módulo 1 | Título do Módulo | 1.1 Subtopico | Descrição |

## Links Rápidos

| Módulo | Teoria | Exercícios | Projeto |
|--------:|:------:|:----------:|:-------:|
| Módulo 1<br>Nome do Módulo | [Teoria](teoria/modulo_01_nome_do_modulo.md) | [Exercícios](exercicios/modulo_01_exercicios_nome_do_modulo.md) | [Projeto](projetos/modulo_01_projeto_nome_do_modulo.md) |

## Planejamento das Aulas

- Ver `planejamento_aulas.md` para uma tabela detalhada.

```

9) Observações finais

- Mantenha a consistência nos nomes de arquivos (use `slugified` nomes em minúsculas com underscores).
- Garanta que todas as referências internas utilizem caminhos relativos consistentes.


- **Planejamento das Aulas:** Criar um arquivo `planejamento_aulas.md` na raiz do repositório contendo:
  - Título: "Planejamento das Aulas - [Nome do Curso]"
  - Tabela detalhada com as colunas:
    - **Aula** (número da aula)
    - **Módulo** (título do módulo)
    - **Conteúdo** (descrição do que será ensinado)
    - **Duração** (tempo estimado)
    - **Arquivos Relacionados** (links para teoria, exercícios e projetos)
  - Exemplo de estrutura da tabela:

    ```markdown
    | Aula | Módulo | Conteúdo | Duração | Arquivos Relacionados |
    |------|--------|----------|---------|----------------------|
    | 1 | Introdução | Conceitos básicos, configuração do ambiente | 60 min | [Teoria](teoria/modulo_01_introducao.md) \| [Exercícios](exercicios/modulo_01_exercicios_introducao.md) |
    | 2 | Fundamentos | Sintaxe básica, variáveis e tipos | 60 min | [Teoria](teoria/modulo_02_fundamentos.md) \| [Exercícios](exercicios/modulo_02_exercicios_fundamentos.md) |
    ```

- **LICENSE:** Criar um arquivo LICENSE (pode ser uma licença padrão como MIT ou Apache 2.0).


## Considerações Adicionais

- Manter a consistência na formatação Markdown e na estrutura de arquivos.
- Garantir que todos os links no sumário e referências de imagens estejam corretos.
- Os exemplos de código devem ser funcionais e claros.
- Os exercícios e projetos devem ser desafiadores, mas alinhados com o nível do módulo.
- **Não utilizar emojis** nos materiais do curso para manter um tom mais profissional e técnico.
