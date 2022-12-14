<h1>
<p align="center">
  <img src="https://github.com/arturo-ugalde/CorretajeSeguros/blob/5eaf422fa61640d9bb88b2fba011a365f66dea28/Documentos/44.png" alt="Logo" width="140" height="110">
  <br>Corretaje de Seguros
</h1>
</p>

Este es el repositorio del proyecto de clustering sobre empresas que maximicen los ingresos de la compañía de corretaje de seguros.

Este proyecto tiene el interés de una  empresa de corretaje de seguro en entender el grupo de empresas que le generan mayores ingresos de acuerdo con  las  características  de cada cliente. Para ello se utilizará la información de facturación histórica de la empresa en la cual se asocia cada  una de  
las cuentas que se han ganado y los ingresos para la compañía.
Buscamos realizar clustering sobre empresas que maximicen los ingresos de la compañía.

La carpeta DatosFuentes almacena el archivo con la información empresarial que será insumo para el análisis en el proyecto.

En la carpeta Codigos encontrará los códigos fuentes utilizado para analizar los datos y aplicar los algoritmos de clustering.
```py
# librerías base
import pandas as pd
from IPython.display import HTML
from IPython.display import display
import matplotlib.pyplot as plt
import seaborn as sns
import numpy as np
from IPython.display import HTML
from IPython.display import display
# cargamos el dataset
data = pd.read_excel('Base seleccion.xlsx')
numericalColumns = data._get_numeric_data().columns.tolist() 
categoricalColumns = list(set(data.columns) - set(data.describe().columns))
data.head()
```
Por último la carpeta Documentos contiene el archivo pdf con la propuesta y resultados del proyecto.

## Resumen General de los datos:
<div  >
<img  src = "https://github.com/arturo-ugalde/CorretajeSeguros/blob/d98efc42782d34ac36366c29850554b0587d0510/Documentos/overview.png"  />
</div>

## Estadísticas descriptivas:
<div  >
<img  src = "https://github.com/arturo-ugalde/CorretajeSeguros/blob/a1c579529a56e1d9a1f684d8ea6bb660e62276f9/Documentos/statistics.png"  />
</div>
