# CI3725
## Traductores e Interpretadores


### <a href="#noticias">Noticias del Curso</a>
### <a href="#preparadores">Preparadores</a>
### <a href="#cronograma">Cronograma</a>
### <a href="#proyecto">Proyecto</a>

----------
## <a name="noticias"></a>Noticias del Curso

#### 04/05/2013 - 01:30pm

**Aclaratoria:** En el enunciado de la primera entrega, la salida del primer ejemplo no corresponde en las lineas y columnas; esto es un error en el enunciado pues las lineas y columnas reportadas deben ser relativas al archivo. 

La salida debería ser:

	TkProgram (Línea 1, Columna 1)
	TkBegin (Línea 2, Columna 2)
	TkDeclare (Línea 3, Columna 3)
	TkId "a" (Línea 4, Columna 4)
	TkComma (Línea 4, Columna 5)
	TkId "b" (Línea 4, Columna 7)
	TkComma (Línea 4, Columna 8)
	TkId "c" (Línea 4, Columna 10)
	TkAs (Línea 4, Columna 12)
	TkInt (Línea 4, Columna 14)
	TkSemicolon (Línea 4, Columna 15)
	TkId "d" (Línea 5, Columna 4)
	TkComma (Línea 5, Columna 5)
	TkId "e" (Línea 5, Columna 7)
	TkComma (Línea 5, Columna 8)
	TkId "f" (Línea 5, Columna 10)
	TkAs (Línea 5, Columna 12)
	TkRange (Línea 5, Columna 14)
	TkId "a" (Línea 6, Columna 3)
	TkEqual (Línea 6, Columna 5)
	TkId "b" (Línea 6, Columna 7)
	TkPlus (Línea 6, Columna 9)
	TkNum "3" (Línea 6, Columna 11)
	TkSemicolon (Línea 6, Columna 12)
	TkRead (Línea 7, Columna 4)
	TkId "e" (Línea 7, Columna 9)
	TkEnd (Línea 9, Columna 1)

#### 03/05/2013 - 10:45pm

* [Casos de prueba para la primera entrega](casos_prueba_e1.tar.gz)
* Las personas en la **[lista](sin_equipo.txt)** no han dado notificación de equipos.

#### 01/05/2013 - 01:19am

* El programa de ejemplo en la seccón **Estructura de un programa** tenía un `;`
  en la última declaración de variables, lo cual es incorrecto. Se actualizó
  la sección sobre la instrucción bloque para aclarar esto.
* No se había aclarado que el espacio en blanco es irrelevante y sólo se
  utiliza para separar tokens. Se ha agregado esta información a la sección
  de **Comentarios y espacios en blanco**.
* Se modificó ligeramente la explicación de la instrucción `case`.
* Se han corregido algunos errores de tipeo.

## <a name="preparadores"></a>Preparadores:

* **Sección 1:** <a href="mailto:hancel.gonzalez@gmail.com">Hancel González</a> 

 **Aula:** AUL009

 **Consulta:** Consultas informales (pasillos o sala de lectura) o previa cita por correo.

 [**Notas**](notas1.pdf)

 [Listado](seccion1.txt)

* **Sección 2:** <a href="mailto:gml.josea2@gmail.com">José Alberto Goncalves</a> 

 **Aula:** AUL010

 **Consulta:** Por correo electrónico.

 [**Notas**](notas2.pdf)

 [Listado](seccion2.txt)

Los dos preparadores anteriores serán los encargados de dar las clases. No obstante, contarán con los dos siguientes para hacer consultas. Y en general, los cuatro corregirán las entregas de sus proyecto.
 
* **Sección 3:** <a href="mailto:chinoxyz@gmail.com">José Sánchez</a> 

 **Consulta:** 

 [**Notas**](http://ldc.usb.ve/~09-10790/notas/notas_traductores_2013_abr_jul.htm)

 [Listado](seccion3.txt)

* **Sección 4:** <a href="mailto:maik302@gmail.com">Michael Woo</a> 

 **Consulta:** 

 [**Notas**](notas4.pdf)

 [Listado](seccion4.txt)

También pueden enviar sus dudas por correo. El correo debe ir titulado **CI3725 - Duda**.

----------
## <a name="cronograma"></a>Cronograma:

Este es el cronograma de preparadurías en caso de que ninguna clase sea suspendida:

<table border="1" align="center">
  <tr align="center">
    <th>Semana</th>
    <th>Fecha</th>
    <th>Tema</th>
  </tr>
  <tr align="center">
    <th>1</th>
    <td>2013-04-22</td>
    <td>No hubo clase de preparaduría.</td>
  </tr>
  <tr align="center">
    <th>2</th>
    <td>2013-04-29</td>
    <td>Introducción al proyecto.<br>Lenguajes Regulares.<br>Expresiones Regulares.</td>
  </tr>
  <tr align="center">
    <th>3</th>
    <td>2013-05-06</td>
    <td><b>Comentarios acerca de la primera entrega</b>.<br>Autómatas Finitos (DFA y NFA).<br>Equivalencias RE-NFA y NFA-DFA</td>
  </tr>
  <tr align="center">
    <th>4</th>
    <td>2013-05-13</td>
    <td>Minimización de Autómatas.<br>Equivalencia DFA-RE.<br>Propiedades de la Clausura de los Lenguajes Regulares.<br>Lema de Bombeo para Lenguajes Regulares.</td>
  </tr>
  <tr align="center">
    <th>5</th>
    <td>2013-05-20</td>
    <td>Lenguajes Libres de Contexto.<br>Gramáticas Libres de Contexto.</td>
  </tr>
  <tr align="center">
    <th>6</th>
    <td>2013-05-27</td>
    <td>Automátas de Pila (PDA).<br>Equivalencias PDA-GLC y GLC-PDA.<br>Lema de Bombeo para Lenguajes Libres de Contexto.</td>
  </tr>
  <tr align="center">
    <th>7</th>
    <td>2013-06-03</td>
    <td>Gramáticas de Atributos.<br><b>Comentarios acerca de la segunda entrega.</b></td>
  </tr>
  <tr align="center">
    <th>8</th>
    <td>2013-06-10</td>
    <td>Cálculos de LookAhead, FIRST y FOLLOW.<br>Condición <i>STRONG LL(1)</i>.<br>Construcción de Tablas LL(1).</td>
  </tr>
  <tr align="center">
    <th>9</th>
    <td>2013-06-17</td>
    <td>Asas y Prefijos viables.<br>Construcción de Tablas LR(0) y SLR(1).<br>Resolución de conflictos: <i>shift-reduce</i> y <i>reduce-reduce</i>.<br><b>Comentarios acerca de la tercera entrega.</b></td>
  </tr>
  <tr align="center">
    <th>10</th>
    <td>2013-06-24</td>
    <td>Máquinas de Turing (MT). <br>MT como: Calculadoras, Reconocedoras y Enumeradoras.<br><b>Comentarios acerca de la cuarta entrega.</b></td>
  </tr>
  <tr align="center">
    <th>11</th>
    <td>2013-07-01</td>
    <td>Lenguajes Recursivos y Recursivamente Enumerables.<br>Propiedades de la Clausura para Lenguajes Recursivos y Recursivamente Enumerables.<br>Problema de la Parada para Máquinas de Turing. </td>
  </tr>
  <tr align="center">
    <th>12</th>
    <td>2013-07-08</td>
    <td>Decidibilidad y Decidibilidad.<br>Complejidad en Tiempo y Espacio.<br>Completitud.</td>
  </tr>
</table>

**Nota:** La planificación puede estar sujeta a cambios.

----------


## <a name="proyecto"></a>Proyecto: 

Intérprete para el lenguaje de programación imperativo **RangeX**. La definición del lenguaje podrá verla en el siguiente <a href="definicion.pdf">vínculo</a>.

Se plantean 4 entregas para el desarrollo de este proyecto:

<table border="1" align="center">
  <tr align="center">
    <th>Entrega</th>
    <th>Semana</th>
    <th>Valor (%)</th>
   
  </tr>
  <tr align="center">
    <td><a href="entrega1.pdf">Enunciado Entrega 1</a></td>
    <td>3</td>
    <td>5</td>
    <td>Analizador Lexicográfico</td>
  </tr>
  <tr align="center">
    <td><a href="entrega2.pdf">Enunciado Entrega 2</a></td>
    <td>7</td>
    <td>8</td>
    <td>Analizador Sintáctico con Árbol Sintáctico Abstracto (AST)</td>
  </tr>
  <tr align="center">
    <td><a href="entrega3.pdf">Enunciado Entrega 3</a></td>
    <td>9</td>
    <td>7</td>
    <td>Tabla de Símbolos y Verificaciones estáticas</td>
  </tr>
  <tr align="center">
    <td><a href="entrega4.pdf">Enunciado Entrega 4</a></td>
    <td>11</td>
    <td>10</td>
    <td>Interpretador con verificaciones dinámicas</td>
  </tr>
<tr align="center">
    <td></td>
    <td></td>
    <th>30</th>
    <td></td>
  </tr>
</table>

Las entregas deben hacerse el día **Viernes** de la semana mencionada antes de las 11:59:59 pm.


----------


#### Reglas del Juego:

0. Deben formar equipos de 2 personas.
1. Cada entrega debe incluir un Makefile, si su proyecto está programado en Haskell.
2. No debe adjuntar los archivos generados por las librerías usadas. 
3. Notificar cual librería, en adición a las recomendadas, usó para el desarrollo de su entrega. Esto incluye la versión y si la misma es complicada de instalar, los pasos de instalación.
4. Asegurese de que su código compile sin errores. Si el mismo no compila, no será corregido.
5. Debe enviar un correo a todos los preparadores, adjuntando el código fuente en un archivo comprimido **tar.gz** de la siguiente manera: **EXGY.tar.gz** donde X es el número (sin el número cero) de la entrega e Y es el número (con el número cero cuando aplique) del grupo asignado. El correo debe titularse **CI3725 - Entrega X Grupo Y**.
6. **Regla del Silencio:** 12 horas antes de la entrega de su proyecto no se aceptarán consultas de ningún tipo y bajo ningún medio.

----------

##### Enlaces de interés:

* [Página Oficial del curso de Teoría](http://ldc.usb.ve/~emhn/cursos/ci3725/201304)

* [Haskell](http://www.haskell.org/haskellwiki/Haskell)

* [Alex](http://www.haskell.org/alex/doc/html/index.html)

* [Happy](http://www.haskell.org/happy/doc/html/index.html)

* [Python](http://docs.python.org/release/2.6.6/)

* [PLY](http://www.dabeaz.com/ply/ply.html)

* [Ruby](http://www.ruby-lang.org/en/downloads/)

* [Racc](http://i.loveruby.net/en/projects/racc/)