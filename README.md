# Octave-MacOSX
Octave Projects Running on Mac OSx.

# Installing from Brew
`brew install octave`

# Crear un ambiente virtual en Python específico para el proyecto
`mkvirtualenv octave`

# Instalando las dependencias correspondientes
Instalando las dependencias que solicita octave que estén instaladas en el ambiente virtual de Python para correr.
```
workon octave
pip install sympy

```

# Instalando paquetes en octave
Desde el terminal, se activa octave y se corren los siguientes comandos:
```
pkg install -forge symbolic
```

# Configurar el ambiente virtual en Octave
Para esto los .m files que se leerán, serán los que están dentro del PATH por default de Octave, o bien, los que se coloquen en una carpeta en el Home("~") llamada **Octave**. Es por esto la línea: addpath ("~/Octave"). Se pueden agregar cuantas direcciones de folders se vayan a necesitar.

### Importante
$USER deberá ser reemplazado por el nombre del usuario corresondiente a su sesión.
```
pkg load symbolic;
setenv PYTHON /Users/$USER/.virtualenvs/octave/bin/python
sympref reset;
syms x;
addpath ("~/Octave");


```