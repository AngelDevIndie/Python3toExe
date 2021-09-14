# Python3toExe

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

- Ejecutar 'python setup.py py2exe'
- El ejecutable se habrá creado en la carpeta 'dist'
