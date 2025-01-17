![Prueba](https://github.com/iFranM18/DIFM23/blob/main/icon/unam_fc_logos.png)

# Aplicación Picket Fence
<div align="justify"> 
Esta aplicación diseñada en App Designer de MATLAB para correr en Windows(86x_64). El programa fue diseñado con la intención de llevar a cabo el análisis de imágenes DICOM obtenidas de la prueba Picket Fence
acorde al TG-142 de la AAPM. Dicha prueba busca corroborar el correcto funcionamiento del colimador multihojas (MLC) mediante un estudio de imagen, en el cuál se buscará detectar anomalías en el posicionamiento
de las mismas mediante software de procesamiento en búsqueda de discrepancias en el posicionamiento del sistema colimador<sub>1</sub>.

<br />
<br />

En esta aplicación se realizó el análisis exhaustivo mediante la plataforma de programación MATLAB, donde se realiza un análsis exhaustivo de dos imágenes DICOM tomadas por un acelerador del fabricante Varian, y una
del fabricante Elekta. La aplicación tiene como objetivo el comparar las posiciones de los pixeles con mayor intensidad con los de su alrededor con la finalidad de encontrar aquellos con la mayor intensidad y 
clasificarlos como 'máximos' respecto al resto, una vez localizado estos 'máximos', el siguiente paso es obtener la desviación estándar de estas posiciones y graficarlas. Como siguiente paso, el programa localiza
el promedio de la desviación estándar, al igual que su máximo, y despliega esta información en una tabla para su rápida visualización. Finalmente, es posible guardar la imagen del análisis y crear un reporte en 
formato .pdf para almacenar la información obtenida del análisis.

</div>

### Requerimientos 


1.- Instalar la aplicación [MATLAB](https://la.mathworks.com/store/?gclid=Cj0KCQiAuqKqBhDxARIsAFZELmI2U62SFmQvDjbBNklz9sMsUFYG39xNu5gLfPHLX4tLkW6P3bT_fBIaAmOsEALw_wcB&ef_id=Cj0KCQiAuqKqBhDxARIsAFZELmI2U62SFmQvDjbBNklz9sMsUFYG39xNu5gLfPHLX4tLkW6P3bT_fBIaAmOsEALw_wcB:G:s&s_kwcid=AL!8664!3!323262175322!p!!g!!get%20matlab&s_eid=ppc_62715811617&q=get%20matlab)  en su versión 2023a/b.

2.- Instalar la aplicación [Picket Fence](https://github.com/iFranM18/DIFM23/tree/main/Picket_Fence_app/Picket_Fence/for_redistribution).

3.- Ejecutar el archivo .exe y esperar a que el proceso de instalación finalice.

4.- Abrir la aplicación Picket_Fence.exe.


### Guía de botones

- Abrir: Este botón abre el directorio donde se encuentra la aplicación para seleccionar la imagen a análizar (Varian/Elekta).

- Cargar imágenes: Al ser presionado, cargará la imagen Elekta o Varian en la gráfica en blanco de la parte superior, así como sus perfiles horizontal y vertical.

- Iniciar análisis: Inicia el proceso de análisis de la imagen seleccionada, desplegando visualmente una imagen interactiva, error promedio, así como la desviación estándar máxima con su par de láminas. 

- Ver imagen original: Checkbox el cual cambia la imagen analizada a la inicial en la gráfica central.

- Guardar imagen: Guarda la imagen.

- Crear reporte: Genera un reporte en archivo .pdf de los resultados en la aplicación.

- Resultados: En esta sección se despliega la información de la desviación estándar y el par de láminas a la que pertenece.

- Cerrar: Finaliza la aplicación.

### Referencias

<a id="1">[1]</a>
Klein, E. E., Hanley, J., Bayouth, J. E., Yin, F., Simon, W. E., Dresser, S., Serago, C. F., Aguirre, F. A., Ma, L., Arjomandy, B., Liu, C., Sandin, C., & Holmes, T. C. (2009). Task Group 142 Report: Quality Assurance of Medical AcceleratorsA). Medical Physics, 36(9Part1), 4197-4212. https://doi.org/10.1118/1.3190392

