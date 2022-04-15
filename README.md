# Spanish nobility titles

A csv file containing the 2823 Spanish nobility titles as of 15/04/2022. The file is called "nobles_de_españa.csv". The collumn headers are: 

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

The data was pulled from <a href="https://www.diputaciondelagrandezaytitulosdelreino.es/guiadetitulo">this website</a>. If you do an empty search it will give you the full list. I just copied the <tbody> element and formated from there. Surprisingly, VScode find and replace (control + h) was enough to remove the horrendus html (see what I mean in the photo) and leave only <tr> to denote a new nobility title and new line for fields. 

The csv uses a plus sign as a separator. Use pd.read_csv(filepath_or_buffer="nobles_de_españa.csv", sep="+") to load a python pandas dataframe.
  
DO NOT USE THIS INFORMATION FOR COMMERCIAL PURPOSES
