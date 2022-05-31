# Modulo 3 (Apuntes)
Tienes una máquina de desarrollo. En esa máquina, es posible que tengas una versión de Python instalada o una versión de una biblioteca que quieras usar. ¿Qué sucede cuando mueves tu programa a una máquina que tiene una versión diferente de Python instalada o diferentes versiones de las bibliotecas de las que depende?

El flujo de trabajo básico se ve así:
+ Crear un entorno virtual que no afecte al resto de la máquina.
+ Ingresar al entorno virtual, donde especifique la versión de Python y las bibliotecas que necesita.
+ Desarrolla tu programa.

## Como correr un Virtual Enviroment
```bash
    cd [directory]
    python3 -m venv env
```

Al crear un VE, se generan la siguiente estructura de carpetas
```
    /env
    |
    +-> /bin
    |
    +-> /include
    |
    +-> /lib
```

Tu entorno necesita el directorio venv para realizar un seguimiento de detalles como qué versión de Python y qué bibliotecas está utilizando. No coloque los archivos de programa en el directorio venv. Te sugerimos que coloques tus archivos en el directorio `src` o algo similar.

## Activar el entorno virtual
En este punto, tienes un entorno virtual, pero no has comenzado a usarlo. Para usarlo, debes activarlo llamando activate a un script en tu directorio env.
```bash
source env/bin/activate
```

## Instalar un paquete
Instalar un paquete mediante pip. El comando pip utiliza el Python Package Index, o PyPi para abreviar, para saber dónde obtener los paquetes. Puedes visitar el sitio web de PyPi para conocer qué paquetes están disponibles.

```bash
pip install [paquete]
```

Para ver qué paquetes están ahora instalados en tu entorno virtual, puedes ejecutar `pip freeze`. Este comando produce una lista de paquetes instalados en el terminal:

``` log
# Mensaje de salida en consola
  python-dateutil==2.8.2
  six==1.16.0
```

## Desactivar el VE.
Simplemente en la misma ruta donde esta el *activate* esta un archivo llamado *deactivate*







