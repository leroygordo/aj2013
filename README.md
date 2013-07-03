# CI3725	
## Traductores e Interpretadores


<table border="1" align="center">
  <tr align="left">
    <th>
        <h3><a href="#noticias">Noticias del Curso</a><br></h3>
		<h3><a href="#preparadores">Preparadores</a><br></h3>
		<h3><a href="#cronograma">Cronograma</a><br></h3>
		<h3><a href="#proyecto">Proyecto</a></h3>
	</th>
    <th align="center" width="500">
<a class="twitter-timeline" href="https://twitter.com/search?q=%23CI3725" data-widget-id="332680065450115073">Tweets sobre "#CI3725"</a>
<script>!function(d,s,id){var js,fjs=d.getElementsByTagName(s)[0],p=/^http:/.test(d.location)?'http':'https';if(!d.getElementById(id)){js=d.createElement(s);js.id=id;js.src=p+"://platform.twitter.com/widgets.js";fjs.parentNode.insertBefore(js,fjs);}}(document,"script","twitter-wjs");</script>
    </th>
  </tr>
</table>

----------
## <a name="noticias"></a>Noticias del Curso

#### 03/07/2013 - 1:00am

Están las [tablas LR(0) Y SLR(1)](parser.pdf) para [miniJSON](gramatica.pdf) y los [pasos de *parseo*](parseo.pdf) de una palabra usando la tabla SLR(1).

#### 02/07/2013 - 10:00am

Se define nuevamente el operador *unión* pues la definida en la [definición](definicion.pdf) del RangeX no es consistente. Quedando ahora:

unión (`a + b`) : toma dos expresiones de tipo `range` y produce un `range`
cuya cota inferior sea igual al mínimo de las cotas inferiores de `a` y `b` y cota superior el máximo de las cotas superiores de `a` y `b`. Por ejemplo: `4..8` + `3..5` = `3..8`.

#### 01/07/2013 - 6:00pm

**[Casos de prueba](casos_prueba_correccion_e3.tar.gz)** usados para la corrección de la entrega 3. Los criterios se los dirá su preparador asignado durante la revisión.

#### 29/06/2013 - 7:30pm

- Publicados [casos de prueba](casos_prueba_e4.tar.gz) para la Entrega 4. **Recordar** que las salidas NO deben imprimirse en archivos sino por pantalla.

- Respecto al anuncio anterior, una variable es inicializada cuando la misma es asignada justo después de ser declarada o es leída a través de un `read`. Este caso no aplica a las variables del `for` pues la misma no puede asignarse ni formar parte de un `read`.

#### 29/06/2013 - 2:00pm

En la última entrega del proyecto se pide reportar los siguientes errores de la verificación dinámica:

		Error: Intento de división por cero.
		Error: Resultado no puede representarse en 32 bits.

Además de los dos tipos de errores que puedan presentarse, deben reportar el siguiente error:
		
		Error: La variable "x" no ha sido inicializada.

Error que ocurre cuando se intenta leer una variable que no ha sido inicializada después de haber sido declarada.

Por otro lado, cuando se consiga el primer error durante la verificación dinámica debe reportarse el mismo y abortar la ejecución del intérprete.

Finalmente, el reporte de errores de su intérprete será de la siguiente forma:

- Si consigue errores durante el análisis lexicográfico, **debe reportarlos todos** y abortar la ejecución de su intérprete.
- De no existir los anteriores pero sí errores durante el análisis sintáctico, **debe reportar el primero** y abortar la ejecución de su intérprete.
- De no existir los anteriores pero sí errores durante la verificación estática, **debe reportar todos (o la cantidad máxima) los errores** y abortar la ejecución de su intérprete.
- De no existir los anteriores pero sí errores durante la verificación dinámica, **debe reportar el primer error conseguido** y abortar la ejecución de su intérprete.

#### 24/06/2013 - 6:45pm

**Anuncio Importante:**

Hubo una tremenda confusión con respecto al alcance de las variables. Consideren este trozo de código en RangeX:

		program
		begin
			declare i as int
			
			for i in 1..3 do 
			begin
				declare i as bool
				...
			end
		end

El código mostrado es totalmente válido. No obstante, si su implementación no contempla las tres declaraciones de la variable `i`, será válido también. 

Disculpe las molestias que esto causaría.

#### 24/06/2013 - 1:45pm

**Fe de Errata:**

- El caso de prueba `p2` tiene un error, y es que la variable de la iteración determinada `x1` se declara antes, esto está mal. No obstante, puedo redeclararse dentro de la iteración determinada.

- El caso de prueba `p4` intenta asignar la variable `i` que pertenece a la iteración determinada, esto está mal.

#### 23/06/2013 - 9:45pm

**Aclaratorias:**

- En el caso de prueba `c4.rgx`, recientemente publicado, el primer error no debe ser reportado.

- Verifiquen en principio los errores que se listan en el enunciado. Si hacen otro tipos de verificaciones deben indicarlo en el `LEEME.txt` y puede que sea considerado para una bonificación.

#### 23/06/2013 - 9:00pm

Están disponibles [casos de prueba](casos_prueba_e3.tar.gz) para la tercera entrega  y sus respectivas salidas.  

**Observaciones:**

- Los casos `p1` y `p2` corresponden a casos válidos sintácticamente. Por lo tanto, sus salidas deben corresponder con la mostrada pero no necesariamente mostrar las variables en el mismo orden.

- Los casos `p3` y `p4` corresponden a casos con errores. Sus salidas no necesariamente deben ser iguales a las mostradas pueden variar dependiendo de su implementación.

#### 22/06/2013 - 3:30pm

Están disponibles los [casos de prueba](casos_prueba_e2.tar.gz) usados para la corrección de la segunda entrega.

**Observaciones:** 

- En p1 cambiar el != por /=
- En p2 cambiar el != por /=
- En p3 coloquen ; al final de las instrucciones del case
- En p3 cambien (i-j .. i+j) por ((i-j) .. (i+j))
- En p3 cambien b = a + a * - a / a; por b = a + a * a - a / a;

#### 09/06/2013 - 9:00pm

**Postergada la segunda entrega** de su proyecto para **mañana Lunes 10 de Junio antes de las 11:59pm**. Aquellas personas que hicieron su entrega deben tomar en cuenta la observación hecha en el anuncio anterior y volver a enviar su entrega.

Se está estudiando la posibilidad de un nuevo plazo de entrega, por favor asistan a la preparaduría para saber en que estado se encuentra su entrega.

#### 09/06/2013 - 9:00pm

La instrucción `case` necesita de un separador justo al terminar la instrucción para una guardia pues esto ha de crear ambigüedad en la formulación de su gramática. Quedando la definición del `case` así:

### Condicional `case`

    case <expresión int> of
      <expresión range> -> <instrucción>;
      <expresión range> -> <instrucción>;
      ...
      <expresión range> -> <instrucción>;
    end

La expresión del `case` debe tener tipo `int` y las expresiones de las guardias deben tener
tipo `range`.

Esta instrucción permite definir rangos y asignar alguna
instrucción a ejecutar cuando un entero pertenezca a alguno de ellos. Para ejecutarla se
evalúa la expresión del `case`, luego se recorre en orden cada una de las expresiones `range`
y se evalúan. Cuando el resultado de alguna de las expresiones contenga el entero calculado
anteriormente, se ejecuta la instrucción asociada. Siempre se evalúan todas las expresiones,
es posible que los rangos se solapen y que se ejecuten más de una de las instrucciones asociadas.
Por ejemplo:

    case x of
	    1..4  -> <instrucción 1>;
		3..10 -> <instrucción 2>;
	end

Si `x` es igual a 1 o 2 sólo se ejecuta la instrucción 1. Si está entre 5 y el 10, sólo se ejecuta
la instrucción 2. Pero si es igual a 3 o 4, como ambos valores se encuentran en los rangos de
ambas expresiones, se ejecutan tanto la intrucción 1 como la instrucción 2, en ese orden.

#### 08/06/2013 - 4:00pm

* Están publicados de nuevo los [casos de prueba](casos_prueba_e2.zip)  para la segunda entrega, los anteriores tenían errores.

* **Precendencias de los operandores:**
	* Precedencia General (de menor a mayor):
		- Operadores lógicos.
		- Operadores relacionales y el `>>` tienen la misma precedencia.
		- Operadores aritméticos y de rangos tienen la misma precedencia.

	* Precedencia de los operadores lógicos (de menor a mayor):
		- `or`
		- `and`
		- `not`
	* Precedencia de los operadores relacionales y el `>>` (de menor a mayor):
		- `>>`
		- `==`, `/=`
		- `<`, `<=`, `>`, `>=`
	* Precedencia de los operadores aritméticos y de rangos (de menor a mayor):
		- `<>`
		- `+`, `-`
		- `*`, `/`, `%`
		- ..
		- `-` unario

	**Recordar:**
	- Puede hacerse uso de paréntesis.
	- No debe chequearse tipos.


#### 08/06/2013 - 12:00am

Están publicados 3 [casos de prueba](casos_prueba_e2.tar.gz) para la segunda entrega con su correspondiente salida.

Consideren:

- Las salidas se muestran en un archivo `pX.output`. No obstante, **no se debe** arrojar un archivo de salida. La salida de su analizador sintáctico debe ser por la salida estándar (por pantalla).

- Se cambió la representación de las instrucciones `write` y `writeln`. En vez de decir, por ejemplo:

		WRITE 
		  expresion: VARIABLE 
					   nombre: a

	Debe decir:


		WRITE 
		  elemento: VARIABLE 
					   nombre: a

	Cambiando `expresion` por `elemento` para evitar confusiones.

#### 06/06/2013 - 6:45pm

Para que el *sistema de precendencias* funcione en su herramienta generadora de analizadores sintácticos es necesario que especifiquen explicitamente el terminal correspondiente al operador. Por ejemplo:

En vez de tener reglas:

		E -> E O E
		O -> + 
		   | -
		   | *
		   | <>
		  ...

Cambie las mismas a:
		
		E -> E + E
		E -> E - E
		E -> E * E
		E -> E <> E
	    ...
 
#### 04/06/2013 - 10:30pm

Fe de Errata y Aclaratorias:

2. Pueden asumir las siguientes precedencias de operadores de rangos, ordenadas de menor a mayor precedencia:
	 	
		<> (intersección)
		+ (unión)
		* (escala)
		.. (construcción)

	Entonces la siguiente expresión:

		10 * a + b <> 5..6

	Se debe interpretar como:

		((10 * a) + b) <> (5..6)

3. No se debe manejar chequeo de tipos, por ejemplo, son válidas expresiones:
		
		a = 4 + true
		if 1 + 3 then 
			read a

4. Dado que no se chequean tipos, la representación del árbol que utilizan el mismo símbolo para distintos tipos, decidan sólo un nombre en `operador`. Por ejemplo, el `+` se usa para las operaciones de **unión** de rangos y **suma**
 de enteros, por lo tanto la información en el árbol es  `operador: más` y no  `operador: unión` o `operador: suma`.

#### 03/06/2013 - 11:30pm

Consideren las siguientes precedencias entre todos los operadores, de menor a mayor:

- Operadores lógicos.
- Operadores relacionales y el `>>`.
- Operadores aritméticos y de rangos.

#### 03/06/2013 - 11:00pm

Respecto a las precedencias de los operadores, he acá dos ejemplos:

1. Los relacionales deben tener mayor precedencia que los lógicos; por ejemplo, si tuviese una expresión de la siguiente forma:

		a < b and c

	Lo más razonable es que primero se evalúe `a < b` y luego el operado `and`.

2. Pueden asumir las siguientes precedencias de operadores de rangos, ordenadas de menor a mayor precedencia:
	 	
		+ (unión)
		<> (intersección)
		* (escala)
		.. (construcción)

	Entonces la siguiente expresión:

		10 * a + b <> 5..6

	Se debe interpretar como:

		(10 * a) + (b <> (5..6))

En próximos anuncios aclararemos la precendencia entre todos los operadores.


#### 01/06/2013 - 12:30am

Las expresiones que involucren los operadores `construcción ..` `unión +` `intersección <>` y `escala *` no necesariamente deben ir entre paréntesis, es decir, `(a .. b)`  es una expresión válida pero no son obligatorios los paréntesis. Se pueden construir expresiones como las siguientes:

	a = 1..6
	b = 2..5 + a
	c = 10 * a <> b

#### 29/05/2013 - 10:05pm

Acá está la **gramática** aumentada con atributos que construyen el AST para [SuperQuery](SuperQuery.pdf). Esperamos sea de ayuda.

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
    <td>Lenguajes Libres de Contexto.<br>Gramáticas Libres de Contexto.<br>Automátas de Pila (PDA).</td>
  </tr>
  <tr align="center">
    <th>6</th>
    <td>2013-05-27</td>
    <td>Equivalencias PDA-GLC y GLC-PDA.<br>Gramáticas de Atributos.<br><b>Comentarios acerca de la segunda entrega.</b></td>
  </tr>
  <tr align="center">
    <th>7</th>
    <td>2013-06-03</td>
    <td>Propiedades de la Clausura de los Lenguajes Libres de Contexto.<br>Lema de Bombeo para Lenguajes Libres de Contexto.</td>
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
    <td>Feriado Nacional</td>
  </tr>
  <tr align="center">
    <th>11</th>
    <td>2013-07-01</td>
    <td>Máquinas de Turing (MT). <br>MT como: Calculadoras, Reconocedoras y Enumeradoras.<br>Lenguajes Recursivos y Recursivamente Enumerables.<br><b>Comentarios acerca de la cuarta entrega.</b></td>
  </tr>
  <tr align="center">
    <th>12</th>
    <td>2013-07-08</td>
    <td><br>Propiedades de la Clausura para Lenguajes Recursivos y Recursivamente Enumerables.<br>Problema de la Parada para Máquinas de Turing.<br>Decidibilidad y Decidibilidad.<br>Complejidad en Tiempo y Espacio.<br>Completitud.</td>
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