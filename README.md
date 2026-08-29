# Generador de cuentas de Discord
Solo para fines educativos. Utiliza Gmailnator y un nombre de usuario aleatorio para generar la cuenta. Prueba de concepto de cómo automatizar la creación de cuentas de Discord sin necesidad de escribir ni hacer clic en botones del navegador mediante XPATH.

## Acerca de
Un script que automatiza la creación de cuentas de Discord. Muestra cómo se pueden crear cuentas automáticamente sin que el usuario escriba nada, a menos que haya un captcha (en el caso de h-Captcha, basta con hacer clic). Verifica automáticamente tu cuenta de Discord por correo electrónico y guarda automáticamente la información de inicio de sesión en `login.txt` con el formato `correo electrónico:contraseña:token`. Solo para fines educativos.

## Características
- Extracción automática de correo electrónico
- Nombre de usuario aleatorio de una lista
- Contraseña aleatoria
- Fecha aleatoria
- Verificación automática de correo electrónico
- Obtención automática del token de Discord y otra información de inicio de sesión
- Compatibilidad con proxy
- Multihilo
## Vista previa
![Imagen](https://i.imgur.com/PSpaUEB.png)

## Uso
1. Puedes personalizar los nombres de usuario editándolos en el archivo discord_usernames.txt.

2. Ejecuta el archivo y usa el modo normal si no tienes experiencia con proxies y multihilo.

### Obtener Python
Si no tienes Python instalado, descárgalo y asegúrate de hacer clic en la opción "Añadir a la ruta" durante la instalación.

### Ejecutar con Python
1. Instala los módulos necesarios
```
Ejecuta requirements.bat
```

2. Para ejecutar el script:

```
Abre discordgenerator.py o ejecútalo con Python desde la línea de comandos
```

#### Compatibilidad con proxies
- Si quieres usar proxies, simplemente pega la configuración de los proxies en config/proxies.txt. Si quieres dejar de usar proxies, elimínalos del archivo .txt. El script comprueba automáticamente si hay proxies al iniciarse. Por ahora, solo se admiten proxies HTTP. Si los proxies no están activos, el script mostrará un error de WebDriver.

#### Modo multihilo
- Usa varias ventanas de Chrome
- Ejecuta esto solo si tienes proxies; de lo contrario, una de tus ventanas de Chrome tendrá un límite de solicitudes.

- No uses más de 6 hilos a menos que creas que tu PC puede soportarlo. Recomiendo usar 2 o 3 hilos.

#### Sin subprocesos
- Solo se usa una ventana de Chrome.

#### Preguntas frecuentes
Si no se abre...
1. Asegúrate de que el archivo chromedriver.exe sea de la misma versión que tu navegador Chrome (en este caso, la versión 91).
2. Descarga la última versión de chromedriver.exe: https://chromedriver.chromium.org/downloads
3. Reemplaza el archivo chromedriver.exe en la carpeta.

¿Dónde puedo encontrar mis cuentas generadas?

1. Se encuentran en la carpeta de salida. Abre login.txt para ver las cuentas que se han generado. 