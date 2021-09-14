# Python3toExe

## Método 1
- Instalar Python 3 descargando de la web oficial.
- Abrir consola de comandos
- Ejecutar 'pip install py2exe'
- Navegar a la dirección 'http://www.py2exe.org/index.cgi/Tutorial'
- Los pasos a seguir son:
- Crear un archivo 'setup.py'
- Editar dicho archivo con el contenido:
```sh
from distutils.core import setup
import py2exe

setup(console=['hello.py'])
```
> NOTA: el archivo 'hello.py' se debe sustituir por tu programa python
- Ejecutar 'python setup.py install'
- Ejecutar 'python setup.py py2exe'
- El ejecutable se habrá creado en la carpeta 'dist'

## Método 2
- Instalar Python 3 descargando de la web oficial.
- Abrir consola de comandos
- Ejecutar 'pip install pyinstaller'
- Ejecutar 'pyinstaller --onefile hello.py"
> NOTA: el archivo 'hello.py' se debe sustituir por tu programa python
- El ejecutable se habrá creado en la carpeta 'dist'

> NOTA: Este archivo será un único archivo, pero los antivirus lo detectan como posible troyano. Hay documentación por la red
para crear nuevas distribuciones y no ocurra esto. https://stackoverflow.com/questions/43777106/program-made-with-pyinstaller-now-seen-as-a-trojan-horse-by-avg

## Método 3
- Instalar Python 3 descargando de la web oficial.
- Abrir consola de comandos
- Ejecutar 'pip install cx-Freeze'
- Navegar a la dirección 'https://www.codeunderscored.com/compile-python-exe/'
- Los pasos a seguir son:
- Crear un archivo 'setup.py'
- Editar dicho archivo con el contenido:
```sh
from cx_Freeze import setup, Executable

setup(name = "HELLO" ,
      version = "0.1" ,
      description = "" ,
      executables = [Executable("hello.py")])
```
> NOTA: el archivo 'hello.py' se debe sustituir por tu programa python
- Ejecutar 'Python setup.py build'
- El ejecutable se habrá creado en 'build/exe.win-amd64-3.9'

## Método 4
- Instalar Python 3 descargando de la web oficial.
- Abrir consola de comandos
- Ejecutar 'pip install auto-py-to-exe"
- Ejecutar 'auto-py-to-exe'
- Se abrirá una pestaña del navegador.
- ![imagen](https://user-images.githubusercontent.com/63190654/133272705-2af390f9-6489-4630-a7a3-15fb469e254b.png)
- Aquí seleccionas el script que quieras convertir.
- Si es onefile ó onedirectory. Hay más opciones que puedes investigar.
- Dar al botón 'Convert .py to .exe' y en la carpeta que hayas configurado tendrás el ejecutable.

> NOTA: Realmente esto es un GUI para el método 2 (pipinstaller), pero más fácil de usar. Si no quieres tener problemas de antivirus, selecciona 'onedirectory'. Será una carpeta con archivos necesarios, pero mucha menos cantidad que los otros métodos.
