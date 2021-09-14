# Python3toExe

## Método 1
- Instalar Python 3 descargando de la web oficial.
- Abrir consola de comandos
- Ejecutar 'pip install py2exe'
- Navegar a la dirección 'http://www.py2exe.org/index.cgi/Tutorial'
- Los pasos a seguir son:
- Crear un archivo 'setup.py'
- Editar dicho archivo con el contenido: (NOTA: el archivo 'hello.py' se debe sustituir por tu programa python)
```sh
from distutils.core import setup
import py2exe

setup(console=['hello.py'])
```

- Ejecutar 'python setup.py install'
- Ejecutar 'python setup.py py2exe'
- El ejecutable se habrá creado en la carpeta 'dist'

## Método 2
- Instalar Python 3 descargando de la web oficial.
- Abrir consola de comandos
- Ejecutar 'pip install pyinstaller'
- Ejecutar 'pyinstaller --onefile hello.py" (NOTA: el archivo 'hello.py' se debe sustituir por tu programa python)
- El ejecutable se habrá creado en la carpeta 'dist'

NOTA: Este archivo será un único archivo, pero los antivirus lo detectan como posible troyano. Hay documentación por la red
para crear nuevas distribuciones y no ocurra esto. https://stackoverflow.com/questions/43777106/program-made-with-pyinstaller-now-seen-as-a-trojan-horse-by-avg
