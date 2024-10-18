#  Guía Completa de Comandos Git

Este documento es una referencia rápida con todos los comandos de **Git** organizados por su utilidad y contexto de uso.

---------------------------

## 1. Comandos básicos de configuración y creación de repositorios

Estos comandos te permiten iniciar un proyecto con Git, configurarlo y clonar repositorios.

- **`git init` (iniciar):**  
  Inicializa un nuevo repositorio de Git en el directorio actual.

- **`git clone [URL]` (clonar):**  
  Clona un repositorio remoto en tu máquina local.

- **`git config --global user.name "Tu Nombre"` (configurar nombre):**  
  Configura tu nombre de usuario a nivel global para que Git lo use en cada commit.

- **`git config --global user.email "tuemail@example.com"` (configurar correo):**  
  Configura tu correo electrónico a nivel global para que Git lo use en cada commit.

- **`git config --list` (listar configuración):**  
  Muestra todas las configuraciones de Git en tu sistema.

---------------------------

## 2. Comandos para hacer seguimiento de cambios

Estos comandos permiten controlar y gestionar los archivos de un proyecto.

- **`git status` (estado):**  
  Muestra el estado del repositorio, qué cambios han sido confirmados y cuáles están pendientes.

- **`git add [archivo]` (añadir):**  
  Añade un archivo específico al área de preparación para confirmarlo.

- **`git add .` (añadir todo):**  
  Añade todos los archivos modificados al área de preparación.

- **`git commit -m "mensaje"` (confirmar):**  
  Confirma los cambios en el historial con un mensaje que describa los cambios.

- **`git commit --amend -m "nuevo mensaje"` (enmienda):**  
  Modifica el último commit, incluyendo un nuevo mensaje o agregando archivos no incluidos.

- **`git diff` (diferencias):**  
  Muestra los cambios entre archivos que no han sido confirmados.

---------------------------

## 3. Comandos de trabajo con ramas

Las ramas son fundamentales para gestionar el flujo de trabajo en Git. Estos comandos permiten crear y gestionar ramas.

- **`git branch` (rama):**  
  Lista todas las ramas existentes en el repositorio.

- **`git branch [nombre]` (crear rama):**  
  Crea una nueva rama con el nombre especificado.

- **`git checkout [rama]` (cambiar de rama):**  
  Cambia a una rama existente.

- **`git checkout -b [nombre]` (crear y cambiar de rama):**  
  Crea una nueva rama y cambia a ella al mismo tiempo.

- **`git merge [rama]` (fusionar):**  
  Fusiona la rama especificada en la rama actual.

- **`git branch -d [rama]` (eliminar rama):**  
  Elimina una rama que ya no es necesaria.

---------------------------

## 4. Comandos para trabajar con repositorios remotos

Estos comandos se utilizan para trabajar con servidores remotos, permitiendo enviar y recibir cambios desde y hacia otros desarrolladores.

- **`git remote` (remoto):**  
  Lista los repositorios remotos configurados.

- **`git remote add origin [URL]` (añadir remoto):**  
  Configura un repositorio remoto llamado `origin`.

- **`git fetch` (obtener):**  
  Descarga los cambios del repositorio remoto, pero no los fusiona con tu código local.

- **`git pull` (jalar):**  
  Combina (fusiona) los cambios del repositorio remoto con tu rama local.

- **`git push [nombre-remoto] [rama]` (empujar):**  
  Envía los commits locales a una rama en el repositorio remoto.

---------------------------

## 5. Comandos para historial y revisión de cambios

Git permite ver el historial de cambios realizados en el proyecto, quién los hizo y qué modificaciones incluyeron.

- **`git log` (registro):**  
  Muestra el historial de commits del proyecto.

- **`git log --oneline` (registro en línea):**  
  Muestra el historial de commits en un formato compacto (solo ID y mensaje).

- **`git show [commit]` (mostrar commit):**  
  Muestra los detalles de un commit específico.

- **`git blame [archivo]` (culpa):**  
  Muestra línea por línea quién realizó los cambios en un archivo.

---------------------------

## 6. Comandos de deshacer cambios

Estos comandos son útiles para corregir errores o deshacer cambios que no deseas mantener.

- **`git reset [archivo]` (reiniciar archivo):**  
  Elimina el archivo del área de preparación, pero mantiene los cambios locales.

- **`git reset --hard [commit]` (reiniciar fuerte):**  
  Vuelve al estado de un commit específico y descarta todos los cambios posteriores.

- **`git revert [commit]` (revertir commit):**  
  Crea un nuevo commit que deshace los cambios de un commit anterior.

- **`git clean -f` (limpiar):**  
  Elimina archivos no rastreados del directorio de trabajo.

---------------------------

## 7. Comandos de colaboración y revisión

Cuando trabajas en equipo, estos comandos te ayudan a coordinar y gestionar los cambios realizados por diferentes colaboradores.

- **`git stash` (guardar temporalmente):**  
  Guarda los cambios actuales de manera temporal sin hacer un commit.

- **`git stash pop` (recuperar cambios):**  
  Aplica los cambios guardados en el stash y los elimina del mismo.

- **`git tag [nombre]` (etiquetar):**  
  Crea una etiqueta en un commit para señalar versiones o lanzamientos importantes.

---------------------------

## 8. Comandos avanzados

Estos comandos son más avanzados, pero útiles para tareas específicas de mantenimiento, reorganización o optimización del historial de cambios.

- **`git rebase [rama]` (reorganizar):**  
  Mueve los commits de una rama sobre otra, manteniendo un historial lineal.

- **`git cherry-pick [commit]` (elegir commit):**  
  Aplica los cambios de un commit específico a la rama actual.

- **`git reflog` (registro de referencia):**  
  Muestra el historial de todas las acciones que Git ha realizado en el repositorio, incluyendo cambios de ramas y commits eliminados.

- **`git bisect` (bisección):**  
  Ayuda a encontrar el commit que introdujo un error, haciendo una búsqueda binaria en el historial de commits.

---------------------------

## 9. Otros comandos útiles

Comandos adicionales que no encajan en las categorías anteriores, pero que son prácticos para tareas comunes.

- **`git shortlog` (registro corto):**  
  Muestra un resumen de commits agrupados por autor.

- **`git archive` (archivar):**  
  Crea un archivo comprimido (tar o zip) de una versión específica del proyecto.

- **`git gc` (recolección de basura):**  
  Optimiza el repositorio limpiando datos innecesarios.

- **`git fsck` (verificación del sistema de archivos):**  
  Comprueba la integridad del repositorio y su base de datos.

---------------------------

## 10. Ayuda y documentación

Si necesitas ayuda con cualquier comando de Git, estos comandos pueden ser muy útiles.

- **`git help [comando]` (ayuda):**  
  Muestra la documentación para el comando especificado.

- **`git --version` (versión):**  
  Muestra la versión de Git instalada en tu sistema.

---------------------------

## 11. Recursos adicionales

https://drive.google.com/file/d/1wl9I1Y0Rj9vXAy3IdfspCVD1HCOkvq6F/view?usp=drive_link
https://www.freecodecamp.org/espanol/news/hoja-de-referencia-de-git-50-comandos-de-git-que-debe-conocer-2/

Este documento cubre los comandos de Git más importantes y sus usos. Documentación oficial: https://git-scm.com/doc 
