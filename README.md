<h1>📌 Parcial Mercado Libre</h1>
Este proyecto permite detectar si un humano es mutante basándose en su secuencia de ADN. El ADN es recibido como un arreglo de Strings, donde cada String representa una fila de una tabla de 6x6. Las letras permitidas en cada fila son: A, T, C, G, que representan las bases nitrogenadas del ADN. Se determina que un humano es mutante, si se encuentra más de una secuencia de cuatro letras iguales, de forma oblicua, horizontal o vertical. 

<h3>📌Nivel 1</h3>
Programa  en java spring boot que cumpla con el método pedido por Magneto utilizando una arquitectura en capas de controladores, servicios y repositorios. 

<h3>📌Nivel 2</h3>
API REST para detectar mutables, en Render: link
<h5>- Metodo y Endpoint: POST → /mutant/</h5>
<h5>- Formato del Body:</h5>
{ "dna": ["ATGCGA", "CAGTGC", "TTATGT", "AGAAGG", "CCCCTA", "TCACTG"] }

<h3>📌Nivel 3</h3>
Devuelve un JSON con el conteo de mutantes y humanos verificados.
<h5>Metodo y Endpoint: GET → /stats/</h5> 
<h5>Formato de respuesta:</h5>
{
  "count_mutant_dna": 40,
  "count_human_dna": 100,
  "ratio": 0.4
}

<h3>📌 Ejemplos para Pruebas</h3>
<h5>- "mutant": true</h5>
{ "dna": ["TGAC", "AGCC", "TGAC", "GGTC"] }
<h5>- "mutant": false</h5>
{ "dna": ["AAAT", "AACC", "AAAC", "CGGG"] }

<h3>📌 Enlaces para Pruebas</h3>
<ul>
  <li>Swagger UI: Si la API está en funcionamiento, puedes realizar pruebas en http://localhost:8080/swagger-ui/index.html.</li>
</ul>


<h3>📌 Diagrama de Secuencia</h3>
