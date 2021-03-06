# MNO-InteractivePLU

Este repositorio es creado para ejecutar los algoritmos de facotización PLU de manera interactiva generados en el examen de computo matricial de la materia métodos numéricos y optimización, disponible en el siguiente [repositorio](https://github.com/mno-2020-gh-classroom/ex-modulo-3-comp-matricial-plu-paola-md/tree/master/src/test_algorithms) **privado**. Dado lo anterior, únicamente se encuentra disponible el repositorio anterior para los usuarios autorizados.


Para ejemplificar dos las herramientas utilizadas en clase para ejecutar código de manera interactiva. En particular, se utilizan `binder` y `google collab`. Para poder generar botones interactivos de dichas herramientos, se generóp este repositorio de carácter **público*.

Para evitar redundancia, se ejemplificará de forma detallada, únicamente la parte de unit testing del proyecto. Sin embargo, también se incluyen los archivos necesarios para poder ejecutar los modulos `.py` como `jupyter notebooks` disponibles en el respositorio original, disponibles en la carpeta `src`.

**Contenidos:**

- El _notebook_ "UnitTestingPLU.ipynb" puede ejecutarse en _google collab_  haciendo click en el siguiente botón: <a href="https://colab.research.google.com/github/C1587S/MNO-interactivePLU/blob/master/UnitTestingPLU.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

### Binder

- El ejemplo utilizando un enfoque modular, y ejecutanto los tests desde la línea de comandos, o usando _magic commands_ desde un _jupyternotebook_  puede ejecutarse dando clicl al siguiente botón: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/C1587S/MNO-interactivePLU/master)

Para ejecutar los test unitarios que garantizan vairas pruebas individuales del correcto funcionamiento del algoritmo, debemos **abrir una nueva terminal** en el entorno de jupyter generador por `binder`.

Posteriormente, entramos al directorio _code_ y ejecutamos los test unitarios dispnibles en el script _test_plu.py_ utilizando `pytest`.

Los comando específicos a ejectuar en la terminal son los siguientes:

```{bash}
$cd code
$pytest -v test_plu.py
```


En particular, debemos observar si cada test pasó o falló si utilizamos la bandera `-v`

Un ejemplo, del test _durante su ejecución_ es el siguiente:

Incluir imagen.


Si queremos que se muestren los stadout intermedios producidos durante ls pruebas, debemos utilizar la bandera `-s`

```{bash}
$pytest -v -s test_plu.py
```
