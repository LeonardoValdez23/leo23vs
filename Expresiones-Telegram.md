# Telegram Bot para Consultas de Uber

Este proyecto es un bot de Telegram que te permite realizar consultas sobre Uber de una ciudad a otra en una fecha específica.

# Expresión regular para detectar preguntas y consultas de Uber:

\b(qué|cuándo|dónde|por qué|cómo)\b|\bUber de (\w+) a (\w+) el (\d{1,2}) de (\w+)

- `\b(qué|cuándo|dónde|por qué|cómo)\b`: Este grupo coincide con palabras como "qué", "cuándo", "dónde", "por qué" y "cómo". El \b representa un límite de palabra para asegurarse de que la palabra esté completa.
- `|`: Es el operador de alternancia, que permite buscar cualquiera de los dos patrones que están a ambos lados del operador.
- `\bUber de`: Esto busca la palabra "Uber" seguida de la palabra "de".
- `(\w+)`: Este grupo coincide con una o más letras, dígitos o guiones bajos, representando el origen del viaje en Uber.
- `a`: Coincide con la letra "a", que separa el origen y el destino del viaje en Uber.
- `(\w+)`: Otro grupo que coincide con una o más letras, dígitos o guiones bajos, representando el destino del viaje en Uber.
- `el`: Coincide con la palabra "el", que introduce la fecha del viaje en Uber.
- `(\d{1,2})`: Este grupo coincide con uno o dos dígitos, representando el día del mes en el que se realizará el viaje en Uber.
- `de`: Coincide con la palabra "de", que separa el día del mes y el mes en palabras.
- `(\w+)`: Otro grupo que coincide con una o más letras, representando el mes en palabras en el que se realizará el viaje en Uber.

![Captura de pantalla del bot](/Users/leonardovaldez/Documents/Leng. y Autom. I/Git-trabajos/tele-bot.png)


## Funcionalidades

- Saludo inicial al iniciar el bot con el comando `/start`.
- Proporcionar ayuda con el comando `/ayuda`.
- Responder a consultas y preguntas sobre Uber.

## Uso

1. Inicia el bot con el comando `/start`.
2. Utiliza el comando `/ayuda` para obtener información sobre cómo interactuar con el bot.
3. Realiza consultas sobre Uber utilizando el formato "Uber de CiudadOrigen a CiudadDestino el DD de Mes".

Ejemplo de consulta: "Uber de México a Japón el 25 de marzo".


## Ejecución

1. Clona este repositorio en tu máquina local.
2. Instala las dependencias necesarias (Telegram API).
3. Ejecuta el script Python `main.py` para iniciar el bot.

## Dependencias

Este proyecto utiliza la librería `python-telegram-bot` para interactuar con la API de Telegram. Asegúrate de instalar esta dependencia antes de ejecutar el bot.

## Contribución

Si deseas contribuir a este proyecto, sigue estos pasos:
1. Haz un fork del repositorio.
2. Crea una nueva rama para tu contribución (`git checkout -b feature/nueva-funcionalidad`).
3. Realiza tus cambios y haz commit (`git commit -am 'Agrega nueva funcionalidad'`).
4. Haz push de tus cambios a tu repositorio (`git push origin feature/nueva-funcionalidad`).
5. Crea un pull request en GitHub para que podamos revisar tus cambios.

¡Gracias por contribuir!

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo LICENSE.md para más detalles.
