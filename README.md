# Spanish nobility titles

DO NOT USE THIS INFORMATION FOR COMMERCIAL PURPOSES

A csv file containing the 2823 official Spanish nobility titles as of 15/04/2022. The file is called "nobles_de_españa.csv". The first row of the file is the collum headers. The collumn headers are: 

'Título',
'Fecha/año concesión título',
'Monarca concesión',
'Grandeza',
'Fecha/año concesión grandeza',
'Monarca Grandeza',
'Concesionario',
'Concesionario Grandeza',
'Sucesivos titulares',
'Titular actual',
'Fecha Carta sucesión',
'Fecha Boe',
'Otros títulos'

The csv uses a plus sign as a separator. If you use Python and Pandas you can load the file as a dataframe with pd.read_csv(filepath_or_buffer="nobles_de_españa.csv", sep="+") (reminder for myself)

The data was pulled from <a href="https://www.diputaciondelagrandezaytitulosdelreino.es/guiadetitulo">this website</a>. If you do an empty search it will give you the full list. I just copied the <tbody> element and formated from there. Surprisingly, VScode find and replace (control + h) was enough to remove the horrendus html (see what I mean in the photo) and leave only <tr> to denote a new nobility title and new line for fields. 

Some individuals have multiple titles. For example, the duque of Abrantes is also the marquess of the Duero. Mantaining the title takes money and gives you no fiscal benefit. If for whatever reason the title has no person to fall to (they are dead or broke or otherwise) the title goes to a "limbo". The king can then "rehabilitate" the line by giving the title to someone else. 
    
To me this is interesting. If you share this opinion try starting with wikipedia: <a href="https://en.wikipedia.org/wiki/Spanish_nobility">spanish nobility</a>, <a href="https://en.wikipedia.org/wiki/Grandee">Grandee of Spain</a>

# Títulos nobiliarios Españoles

NO UTILIZES ESTA INFORMACIÓN PARA FINES COMERCIALES
    
Un archivo csv que contiene los 2823 nobles españoles, tal y como vienen en la <a href="https://www.diputaciondelagrandezaytitulosdelreino.es/guiadetitulo">Diputación Permanente y Consejo de la Grandeza de España y Títulos del Reino</a> (15/04/2022). El archivo se llama "nobles_de_españa.csv". La primera fila del mismo define los nombres de la columna, que son:
    
'Título',
'Fecha/año concesión título',
'Monarca concesión',
'Grandeza',
'Fecha/año concesión grandeza',
'Monarca Grandeza',
'Concesionario',
'Concesionario Grandeza',
'Sucesivos titulares',
'Titular actual',
'Fecha Carta sucesión',
'Fecha Boe',
'Otros títulos'
 
El archivo csv utiliza un signo más "+" como separador. Si utilizas pyhton y pandas puedes cargar el archivo como un dataframe con pd.read_csv(filepath_or_buffer="nobles_de_españa.csv", sep="+") (reminder for myself)

Si realizas una busqueda sin nada en la web dada obtendras la tabla de la cual he sacado los datos. Simplemente he copiado el elemento <tbody> y lo que formateado a mi gusto. Sorprendentemente la opción de buscar y reemplazar de VScode (control + h) fué suficiente para quitar el html horrendo (ve la captura de pantalla asociada) y dejar solo <tr> para marcar diferentes títulos y nueva linea para diferentes campos. 

Algunos nobles tienen multiples títulos. Por ejemplo el duque de Abrantes es también el marqués del Duero. Mantener un título cuesta dinero y no da ninguna ventaja fiscal. El Rey puede elegir rehabilitar una linea en una nueva persona, lo que también cuesta dinero. 
    
Algunas referencias para leer más sobre esto: <a href="https://en.wikipedia.org/wiki/Spanish_nobility">spanish nobility</a>, <a href="https://en.wikipedia.org/wiki/Grandee">Grandee of Spain</a>  

<img src="https://github.com/villarjorge/spanish_nobles/blob/main/Horrible_html.png" alt="horrendus html">
