# `Proyecto Selenium`

**_`Índice`_**   
1. [_`Marcación Creditos Colpatria Modulo Garantias`_](#id1)
1. [_`Pre-requisitos`_](#id2)
    1. [_`Librerías`_](#id1_1)  
    1. [_`Archivo Inicializar.py`_](#id1_2)          
1. [_`Comenzar`_](#id3)
1. [_`Construido con`_](#id4)
1. [_`Autores`_](#id5)
1. [_`Expresiones de Gratitud`_](#id6)

## _`Marcación Creditos Colpatria Modulo Garantias`_<a name="id1"></a>

_Proyecto de pruebas automatizadas con Selenium para validar aplicativo de marcar obligaciones (créditos) correspondientes a los segmentos de Colpatria Garantías y Expediente Virtual de acuerdo con bases suministrada por el Banco para que dichas obligaciones/créditos no puedan ser solicitados por página por ningún funcionario de Banco y sean marcadas como "CUSTODIA LEGAL HOLD"._

## `Pre-requisitos` 📋<a name="id2"></a>

### `Librerías`<a name="id1_1"></a>
_Se debe tener instalado python y el paquete pip adicional a esto se debe instalar los siguientes componentes mediante el archivo_ __requirements.txt__ _con el siguiente comando_ **`pip install -r requirements.txt`**




|                                   |             LIBRERIAS             |                                   |                                   |
|-----------------------------------|-----------------------------------|-----------------------------------|-----------------------------------|
|      allure-python-commons        |          atomicwrites             |               attrs               | backports.entry-points-selectable |
|             behave                |             colorama              |               distlib             |            et-xmlfile             | 
|            filelock               |            imap-tools             |         importlib-metadata        |              jdcal                | 
|         more-itertools            |           platformdirs            |             parse-type            |            packaging              |
|              parse                |            openpyxl               |               pluggy              |            psycopg2               |
|              py                   |            pyodbc                 |               pyparsing           |              pytest               |
|              selenium             |            six                    |               requests            |      unittest-xml-reporting       |
|              urllib3              |          virtualenv               |               wcwidth             |                 zipp              |



### `Archivo Inicializar.py`<a name="id1_2"></a>
_Crear un archivo_ **`Inicializar.py`** _ubicado en la  siguiente ruta `src\functions\` con la siguiente estructura y agregar los parametros de conectividad necesarios o configuraciones personalizadas que requiera el ambiente segun el equipo_
~~~
import os

class Inicializar():
    # Directorio Base
    basedir = os.path.abspath(os.path.join(__file__, "../.."))
    DateFormat = '%d/%m/%Y'
    HourFormat = "%H%M%S"

    # JsonData
    Json = basedir + u"/pages"
    # BROWSER DE PRUEBAS
    NAVEGADOR = u'CHROME'
    # DIRECTORIO DE LA EVIDENCIA
    Path_Evidencias = basedir + u'/data/capturas'
    # HOJA DE DATOS EXCEL
    Excel = basedir + u'/data/ArchivoConfig.xlsx'
    Environment = 'QA'

    if Environment == 'QA':
        URL = ''
        URL_DEUDOR = ''
        URL_TOKEN = ''
        URL_CASOS =''
        DB_HOST = ''
        DB_PORT = ''
        DB_DATABASE = ''
        DB_USER = ''
        DB_PASS = ''
        USER_TOKEN = ''
        PASSWORD_TOKEN = ''
        APLICATION_TOKEN = ''
        RUTA_CHROME = 'C:\\Program Files (x86)\\Google\\Chrome\\Application\\chrome.exe'
        MAILUSER = ''
        MAILPASSWORD = ''
~~~

_Crear ambiente virtual en la raiz del proyecto con el comando_ **`python -m virtualenv enviroment`** ó **`python -m venv enviroment`** _Seguido a esto activarlo ejecutando el archivo activate.bat ubicado en la ruta `enviroment/Scripts` o ejecutando el siguiente comando en la terminal_ **`./Enviroment/Scripts/activate.bat`**
 

## Comenzar 🚀<a name="id3"></a>

_Desde visual Studio code puedes ejecutar el archivo:_ **projectSeleniumInmofianza.py**
_o activar el entorno virtua por consola y ejecutar el archivo antes mencionado_


## `Construido con` 🛠️<a name="id4"></a>

_El presente proyecto esta construido en lenguaje python con la libreria de webdriber de Selenium_


## `Autores` ✒️<a name="id5"></a>

* **Daniel Duran** - *Analista QA* - [DaniDuran](https://github.com/DaniDuran)


## `Expresiones de Gratitud` 🎁<a name="id6"></a>


