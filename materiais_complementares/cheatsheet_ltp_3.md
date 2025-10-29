# Cheatsheet - LTP 3

## HTTP
- `GET /recurso` -> leitura, sem efeitos colaterais.
- `POST /recurso` -> cria/processa novos dados.
- `PUT /recurso/{id}` -> cria ou substitui recurso.
- `DELETE /recurso/{id}` -> remove recurso.

## Servlet Essentials
```java
@WebServlet("/path")
public class ExemploServlet extends HttpServlet {
  @Override
  protected void doGet(HttpServletRequest req, HttpServletResponse resp) throws IOException {
    resp.setContentType("text/plain");
    resp.getWriter().write("Hello servlet");
  }
}
```
- `init()` -> inicializacao.
- `destroy()` -> limpeza de recursos.
- `req.getParameter("nome")` -> parametro.
- `req.getSession()` -> sessao.

## JSP / JSTL
- Diretiva: `<%@ page contentType="text/html; charset=UTF-8" %>`
- EL: `${usuario.nome}`
- Loop: `<c:forEach var="item" items="${lista}">...</c:forEach>`
- Condicional: `<c:if test="${empty lista}">Sem dados</c:if>`
- Include dinamico: `<jsp:include page="/WEB-INF/views/cabecalho.jsp" />`

## MVC Flow
1. Servlet recebe requisicao.
2. Chama servico/DAO.
3. Seta atributos `req.setAttribute("dados", valor)`.
4. Encaminha: `req.getRequestDispatcher("/WEB-INF/views/pagina.jsp").forward(req, resp);`

## Boas Praticas
- Separar logica de negocio (Servico) de logica de apresentacao (JSP).
- Utilizar DAOs para lidar com persistencia.
- Validar entradas no servidor e no cliente.
- Configurar codificacao UTF-8 em todas as respostas.
