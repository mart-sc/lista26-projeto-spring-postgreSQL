# Lista 26 - Projeto Spring com PostgreSQL
- Projeto desenvolvido no curso DEV-TI Unoesc

## Como rodar
- Tenha o PostgreSQL e seus drivers instalados:

- URL: jdbc:postgresql://localhost:5432/empresa
- username: postgres
- password: postgres
	
- Tenha o STS instalado, depois importe o projeto e dê start na "lista26"
- Ele irá iniciar o servidor do Tomcat na porta 8080
- Você poderá acessar "localhost:8080/" e o "localhost:8080/index_ajax_tabela.html" no seu navegador

## Lista de endpoints
- localhost:8080/api/funcionarios -> lista todos os funcionários registrados (GET)
- localhost:8080/api/funcionarios/listar-paginas -> lista todo conteúdo paginado (GET)
- localhost:8080/api/funcionarios/{id} -> busca funcionário pelo ID (GET)
- localhost:8080/api/funcionarios/xml/{id} -> busca funcionário pelo ID e resultado é mostrado em XML (GET)
- localhost:8080/api/funcionarios/buscar?nome={nome} -> busca funcionário pelo nome (GET)
- localhost:8080/api/funcionarios/faixa-salarial?minimo={valor1}&maximo={valor2} -> lista funcionários de salário entre valor1 e valor2 (GET)
- localhost:8080/api/funcionarios/dependentes -> lista todos funcionários que possuem dependentes (GET)
- localhost:8080/api/funcionarios/ -> Inclui funcionário. OBS: Requer o corpo da requisição, utilize o Postman (POST) 
- localhost:8080/api/funcionarios/{id} -> Atualiza funcionário. OBS: Requer o corpo da requisição, utilize o Postman (PUT)
- localhost:8080/api/funcionarios/{id} -> Deleta funcionário. (DELETE)

## Tecnologias
- Spring Tool Suit 4
- H2 Database para testes (banco em memória)
- PostgreSQL
- HTML, CSS, JavaScript
- JQuery (com EasyAutoComplete) e Bootstrap