# Sección 7: GitHub - Básico

## Introducción a la interfaz de GitHub

-   fork: hacer un fork en github es clonar un repositorio a mi propio github para por ejemplo poder modificarlo a mi gusto, sin pedir permiso a nadie
-   issue: problemas, sugerencias, bug fixes o cualquier pregunta (que cualquier usuario) que pueda hacer a este repositorio. sirve para hacer **seguimiento a un proyecto**
-   **pull request**: hay varias explicaciones para esto. una de estas es que por ejemplo yo clone el repo y solucione un bug... entonces mediante el pull request podemos hacer cambios en un repo que no nos pertenece, como por ejemplo el re react. o por ejemplo si tienes un junior en el que no confias puedes decirle que clone el repo, haga los cambios y solicite o envie un pull request.
-   actions: acciones automaticas que se pueden ejecutar en ciertas condiciones, por ejemplo cuando subo algo.
-   projects: gestor de proyectos
-   wiki: es como crear una especie de repositorio o wiki informativo para que la gente lo lean, etc.
-   security
-   insigths: cuantas personas hacer forks, graphs, commits, etc...

## Documentación sobre el Markdown de GitHub

Documentación sobre el Markdown de GitHub  
Markdown de GitHub

Tutorial de Markdown: https://markdowntutorial.com

GitHub Markdown sheet: GitHub Markdown Style Sheet https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

https://import.cdn.thinkific.com/643563/courses/1870146/markdowncheatsheetonline-220524-152537.pdf

Emojis de GitHub: Emojis https://www.webfx.com/tools/emoji-cheat-sheet/

## Buscando archivos en GitHub

**buscar archivo**
El campo de `Go to file` es muy poderoso. Te permite buscar archivos en todo tu repo, rapidamente.

Copy path de github, en combinacion con ctrl + P en vscode es util también
El permalink es un link a un archivo especifico en GitHub

## Raw, Blame, History, Edit and Delete

-   Raw: muestra el archivo en crudo (texto plano)
-   **Blame**: nos muestra una especie de historial de cambios del archivo donde podemos ver quiénes lo hicieron y qué hicieron  
    Si le das click a "blame prior to change" viajarás a esa posicion en especifico. te llevará al commit de ese punto en el tiempo... donde hiciste ese cambio, con los archivos de ese commit
-   History: muestra los commits donde ese archivo se modifico. (esto aplica para cuando buscas el historial de commits de tu repositorio (por ejemplo repo test-curso-gitDevTalles)... y también aplica o se puede usar cuando estas en un archivo y quieres ver los commits donde fue actualizado ese archivo (por ejemplo repo test-curso-gitDevTalles/README.md))
<!-- ! si en algun cambio aparece tu fotografia, y no aparece verificado... es posible que no seas tu -->

## Creando un nuevo archivo en GitHub

un pull request es una rama que se desprendio de cierto punto del tiempo de la rama principal... y cuando queremos unir la rama lo podemos hacer mediante un pull request. la idea de este PR es que nos sirva para hacer un analisis (revision) previo a un merge.

<!-- ! recuerda que todo esto sucede dentro de github -->

si añades un archivo o cambias alguno desde github y en vez de mandar un commit a la rama principal... **creas una nueva rama para ese commit e inicias un pull request** `commit changes`. luego te lleva a otra pagina para que especifiques datos de ese nuevo commit, y le das a `create pull request`.ahora se agrega una nueva rama y un pull request...

al entrar en tu pr puedes comentar, debatir, ver el commit, files changed, etc... ademas de ver el estado de conflictos de tu rama... y tienes 3 opciones para resolver tu PR:

-   create a merge commit
-   squash and merge: tomare los cambios y los unire o acoplaré al ultimo commit realizado (sin crear un nuevo commit)
-   rebase and merge

si haces tu merge... la rama (anterior, del cambio) seguira existiendo, a menos que la borres, o podrias continuar trabajando desde ahi

ahora ya puedes ir a tu carpeta local y hacer un `git pull`

## Git Fetch

supongamos que hiciste 3 cambios en github (o alguien los hizo) creando 3 commits nuevos... y no quieres hacer un pull request o un merge o rebase para no crear un nuevo commit, etc etc...

**como hago para obtener (en mi repo local) las referencias de mi repo remoto?**

-   `git fetch`: las referencias remotas que hiciste se actualizarán... pero te seguiras manteniendo en el mismo lugar (HEAD) en el que estabas
<!-- checa git lg -->
-   para combinar tus cambios al ultimo commit de la rama principal solo haces un git pull y te saldra tu fast forward

## Comentarios en los commits

puedes añadir comentarios propios de gihub en cualquiuer linea de tu codigo.

-   pero solo en la vista del commit... para ello entra al ultimo commit de dicho archivo (solo dale click al enlace de la parte derecha del nombre del archivo, ese es el ultimo commit donde fue modificado)

## Comprender el flujo de GitHub

https://blog.mergify.com/understanding-the-github-pull-request-workflow/

## Bonus - No hacer esto

NUNCA coloques en configuracion las credenciales de usuario de otro usuario...  
porque cuando hagas un commit con dichas credenciales, en github saldra el perfil de dicha persona, a veces pudiendo redirigir a su propio perfil.
**COMO ME DOY CUENTA SI ESA PERSONA REALMENTE ES LA QUE CAMBIO EL CODIGO?**

-   CUANDO LA ETIQUETA **VERIFIED** ESTE COLOCADA, ENTONCES ES AUTENTICO EL CAMBIO. SINO, PUES NO
