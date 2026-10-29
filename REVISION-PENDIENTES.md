# Revisión del documento principal

Se modificaron Protocolo.tex y los capítulos que incluye. Protocolo-revision.tex y las versiones de respaldo no se utilizaron como documento principal.

## Cambios realizados

- Sustitución de los códigos de pose por nombres del ligando y del tipo de acoplamiento. Correspondencia indicada por la autora: pose61 = C60(Gly)4 alostérico; pose72 = C60(Gly)4 de acoplamiento ciego con AutoDock Vina; pose03 = 246DA ortostérico; pose01 = derivado de benzamida alostérico; pose51 = C60(Gly)4 ortostérico.
- Corrección de las asignaciones contradictorias del texto, captions de figuras, referencias escritas con números fijos y referencias sin destino.
- Corrección del caption de DCCM y explicación de sus paneles; corrección de la posición del sistema ciego en el PCA.
- Adición de caption, etiqueta y referencia al esquema del planteamiento. Corrección del caption del mapa epidemiológico y de la figura de estructura del C60.
- Revisión de ortografía, concordancia y explicaciones; separación entre puntuaciones de acoplamiento y actividad experimental.
- Corrección del signo de 0.074 kcal/mol para el primer conjunto de isómeros, de la identificación del fulereno sin glicina en la tabla de potencial electrostático y de la descripción de RMSF de acuerdo con la gráfica.
- Organización de los antecedentes dentro de un mismo capítulo, inclusión de la introducción en el índice y colocación del cronograma antes de los apéndices, ahora identificados como A y B. La numeración de figuras se recalcula automáticamente por capítulo.
- Incorporación de la referencia bibliográfica faltante de Frimayanti y de fuentes verificadas para las correcciones sobre vacunas, fase crítica y puntuaciones de Vina.
- Ajuste de tamaño de DCCM, PCA y FEL y de la tabla epidemiológica para evitar desbordamientos.

## Datos que necesitan confirmación de la autora

1. **Grado y tipo de documento.** La primera portada indica maestría y tesis; la segunda indica doctorado y protocolo. El cronograma se refiere al doctorado y a actividades de 2027–2028. Se conservaron estos datos para no decidir el grado académico sin confirmación.
2. **Imágenes de acoplamiento ciego y alostérico.** `imagenes/Resu/ciego.pdf` repite visualmente `repor-c60.pdf`, con los contactos que acompañan al sistema alostérico. Se retiró únicamente su inclusión como imagen del sistema ciego; ambos archivos originales se conservaron. El sistema ciego conserva su diagrama de contactos. Hace falta una representación 3D comprobada de ese sistema si se desea añadirla.
3. **Paisaje de energía libre.** Los paneles (a) y (e) de `fel.pdf` parecen duplicados, pese a que sus PCA temporales difieren. Se conservó la imagen, se señaló el problema en el texto y se evitó atribuirle una conclusión física. Revisar el script y las trayectorias que generaron esos paneles.
4. **Ramachandran.** El archivo inicial evalúa 237 residuos y el posterior a NPT evalúa 121. No se puede afirmar una mejora directa entre estas selecciones distintas. Verificar cadenas, residuos y archivos usados.
5. **Preparación y campo de fuerza.** Materiales y métodos menciona CHARMM-GUI y GROMOS 54A7, mientras que resultados menciona CHARMM36. Se retiró la atribución contradictoria a AlphaFold de resultados, siguiendo la descripción metodológica. Confirmar el programa de reconstrucción, el campo de fuerza de cada etapa, el modelo de agua y los parámetros del ligando con los archivos de simulación; no se inventaron nuevos parámetros.
6. **Benzamida.** El texto original atribuye la selección tanto al grupo de -6.70 como al de -6.00 kcal/mol y menciona un contacto con Gly133 ausente de la tabla de ese sistema. Se conservan los valores reportados y se señala la necesidad de comprobar la selección. Confirmar también la identidad química exacta del derivado.
7. **Proteína libre.** Los primeros perfiles de RMSD, radio de giro y SASA difieren de los perfiles comparativos posteriores. Confirmar si provienen de la misma trayectoria, referencia y selección de átomos. No se sustituyeron datos de una gráfica por los de otra.
8. **Epidemiología.** El mapa no contiene año o semana de corte y la tabla 2025–2026 no tiene una fuente verificable identificada en el documento. Se conservaron las cifras con esa limitación explícita. DCSA + DG no es el total de casos confirmados; se corrigió el encabezado.
9. **Rotulación dentro de imágenes.** Algunas gráficas ya exportadas contienen `NS2-NS3` en vez de `NS2B-NS3`, `Ciego` como abreviatura y otros detalles tipográficos. El texto y los captions aclaran los sistemas; para cambiar las letras dentro de los gráficos científicos conviene regenerarlos desde sus fuentes, sin alterar curvas ni datos. Las leyendas y distancias de varias representaciones 3D también deben contrastarse con sus tablas.
10. **Bibliografía y datos no verificables.** Se corrigieron referencias claramente ajenas al tema y la entrada ausente, pero esta revisión no certifica todas las cifras publicadas ni sustituye una auditoría de cada artículo. Persisten notas previas sobre fuentes pendientes en los comentarios del código. Debe confirmarse la revisión de Gaussian y la procedencia de las imágenes adaptadas antes de entregar la tesis.

## Verificación

El documento se compiló con latexmk/pdflatex y BibTeX. No quedaron referencias o citas sin resolver, etiquetas duplicadas, códigos de pose visibles ni avisos de cajas que excedan los márgenes. Se revisaron visualmente las páginas de las figuras corregidas. Persisten avisos tipográficos menores de sustitución de fuentes y marcadores PDF, sin impedir la compilación.

## Respaldo

Los archivos previos y el PDF original están en `respaldo-correccion-20261022-162523/`, dentro de esta carpeta.

## Fuentes comprobadas para correcciones puntuales

- OMS, recomendaciones de vacunas: https://www.who.int/publications/i/item/who-wer-9918-203-224
- CDC, fases clínicas: https://www.cdc.gov/dengue/hcp/clinical-signs/index.html
- Trott y Olson, AutoDock Vina: https://pmc.ncbi.nlm.nih.gov/articles/PMC3041641/
- Frimayanti et al., compuesto 246DA: https://pmc.ncbi.nlm.nih.gov/articles/PMC3083692/
