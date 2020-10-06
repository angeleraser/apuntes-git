# Pasos para crear una Key SSH de Github.
1 - Crear una carpeta ruta para guardar las Keys.
2 -Ejecutar en la terminal >> ssh-keygen -t rsa -C "angeleraser@gmail.com".
3 - Copiar la Key con el comando ``` cat "ruta del archivo .pub" ```
4 - Ir a Github > Profile > Settings > SSH Keys y guardar la Key generada.

# Configuracion SSH en Windows
Usando Git Bash seguir los siguientes pasos:
1. Crear una carpeta para guardar las llaves en el disco C para evitar problemas de rutas.
2. Ejecutar el comando `ssh-keygen -t rsa -C "email@example.com"`.
 El correo debe ser el mismo que esta registrado en Github.
 3. Iniciar ssh-agent en background ejecutando el comando `eval "$(ssh-agent -s)"`.
 4. Agregar la llave ssh generada a ssh-agent ejecutando el comando `ssh-add "ruta del archivo .pub"`.
