## Tarea
1. Explicar cuantas maneras existen para vincular HTML con CSS
2. Explicar con sus palabras el conjunto de reglas de CSS (Selector, propiedad, y valor)
3. Explicar los 4 conceptos importantes con ejemplos (selectores, herencia, cascada y especificidad)


La explicación esta en el codigo de la pagina index.html



        <article>
            <h2 id="ManerasVincular">Maneras de vincular HTML con Css</h2>
            <p> Hay 3 maneras:</p>

            
            <ol>
                <li> Utilizando la etiqueta: <"style> h{color:black} <"/style"> </li>
                
                <style>
                    h2{
                        color: grey;
                    }
                </style>
            
                
                <li> Colocando el estilo inline <"h1 style="font-weight: bolder; font-size:3em">CSS Lección 1<"/h1></li>
                <li> Creando una hoja externa, para esto se debe vincular utilizando:
                    <p>
                        Esto se coloca en el head del html
                        <"link rel="stylesheet" href="./styles.css">
                    </p>
                    <p>
                        Se crea el archivo style.css, donde se coloca h1{color:black}
                    </p>
                </li>
            </ol>

        </article>




       <article>
            <h2 id="ConjuntReglas">Conjunto de reglas de CSS</h2>

            <table>
                <thead>
                    <tr>
                        <th>Elemento</th>
                        <th>Definicion</th>
                </thead>
                <tbody>
                    </tr>
                    <tr>
                        <th>Selector</th>
                        <th> Manera de nombrar a los elementos de html para poder estilizarlos</th>
                    </tr>

                    <tr>
                        <th>Propiedad</th>
                        <th>Es el atributo estilistico de cada elemento</th>
                    </tr>

                    <tr>
                        <th>Valor</th>
                        <th>Estilo que tendra la propiedad</th>
                    </tr>
                </tbody>
            </table>


        </article>


        <article>
            <h2 id="ConceptosImportantes">Conceptos Importantes de CSS</h2>

            <ul>
                <li class="conceptos">Selectores:
                    <p>Los selectores son los elementos de HTML, estos son los h de encabezados, tables, img, p, entre otros</p>
                </li>
                <li class="conceptos">Herencia:
                    <p>La herencia es un pilar de CSS que indica que si a un elemento que agrupa varios otros, se le pone un estilo, sus hijos tendran el mismo estilo, no siempre se cumple en caso el estilo no sea heredable</p>
                <p>
                    Ejemplo de aplicación de herencia:
                </p>
                    <p>
                        table{
                            padding: 2%;
                            
                            font-family: 'Courier New', Courier, monospace;
                            width: 50%;
                        }
                    </p>
                    <p>
                        th, tr{
                            border: 2px solid;
                            border: 1px solid;
                        }
                    </p>
                
                </li>
                <li class="conceptos">Cascada:
                    <p>Para aplicación de estilos en los que estos sean de la misma prioridad de aplicación, se eligira el que se haya puesto ultimo en el codigo</p>
                </li>

                <p>Ejemplo de aplicación de cascada:</p>
                <p>
                    th, tr{
                        border: 2px solid;
                        border: 1px solid;
                    }
                </p>

                <li class="conceptos" id="ultimoConcepto">Especificidad:
                    <p>Cada tipo de selector tiene una prioridad, el de mayor numero es el más prioritario</p>
                    <table>

                        <tr>
                        <th>Etiqueta </th>
                        <th> Clases</th>
                        <th> id</th>
                        <th> inline</th>
                        <th>!important </th>
                        </tr>
                        
                        <tr>
                        <th>1 </th>
                        <th> 10</th>
                        <th> 100</th>
                        <th> 1000</th>
                        <th>infinito </th>
                        </tr>
                        
                        
                        </table>
                </li>
            </ul>

            <p>
                Utilizo estos estilos en la hoja externa CSS para mostrar ejemplo de especificidad, asi demostramos la prioridad de id:
            </p>
            <p>
            .conceptos{
                font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            }
            </p>
            <p>
            #ultimoConcepto{
                color: blue;
            }
            </p>
        </article>