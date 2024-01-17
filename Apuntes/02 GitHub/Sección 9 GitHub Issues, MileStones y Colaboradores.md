# Sección 9: GitHub Issues, MileStones y Colaboradores

## Introducción a la sección - Issues

Los colaboradores tienen permiso de edicion y lectura.
Si mi repositorio es publico cualquier persona puede verlos, clonarlos y hacer un pull request. Si es publico es porque quieres contribuir al mundo con algo.

## GitHub Issues

un issue es como una pregunta: se pueden usar para preguntar como funciona esto, o por ejemplo para pedir una nueva caracteristica, o comentarles cualquier cosa.

Cualquier persona puede crear un issue

## Cerrar un issue

Puedes cerrar el issue con el botón "Closed issue"... asi ya no se podran enviar mensajes

-   A parte también puedes bloquear la conversación para que ya no se siga.
-   También puedes borrar dicho issue entrando y dandole a "delete issue"... **PERO** posiblemente no puedas recuperar ese numeral asi que ten presente eso

Cuando por ejemplo editas tu codigo por los comentarios de algun issue:

-   En las lineas añadidas o modificadas de dicho archivo en dicho commit puedes agregar un comentario referenciando (con un link) pegado en dicho issue (por ejemplo #3) diciendo que fue solucionado o agregado.
-   También puedes referenciar (con un link) tus commits, simplemente pegandolos (el HASH version corta... la version larga ya no existe creo) en tu issue resuelto

## Cerrar mediante un commit

si tienes un issue en github... haces las ediciones necesarias en local y luego puedes ser capaz de cerrar dicho issue mediante el commit que realizarás:

-   `git commit -am "Fixes #5: Hecho, borre a la capitana marvel"`: en el numeral debes colocar exactamente el numero de tu issue
-   luego haces `git push`
-   si ves tu issue, automaticamente se habrá cerrado

## Issue templates

puedes crear issue templates en github desde la configuracion de cada repositorio (los configuras **y le das a propose changes para crear un nuevo commit**)... **ahora tendrás disponible dichos templates en la pestaña issues para ser usados**

esto es util por ejemplo cuando tu app esta sufriendo demasiados bugs y las personas pueden usar estos templates

## Labels - Etiquetas

Existen labels o etiquetas predeterminadas dentro de los issues.

-   al momento de crear un issue, **a la derecha puedes aplicarle un label**
-   al ver todos tus issues puedes filtrarlos por etiquetas

Para ver las etiquetas por defecto, dentro de la pestaña "issues"... abajito (al costado de new issue) podras ver una pestañita de **Labels**
También puedes añadirle labels a tus issue templates

## Milestones - Un punto importante

docs: https://docs.github.com/en/issues/using-labels-and-milestones-to-track-work/about-milestones

milestone: algo importante que queremos que pase... por ejemplo un hito. **digamos que también funciona en github como un conjunto o agrupador de issues** o grupo de cosas que se necesitan hacer

es util por ejemplo cuando quieres marcar el lanzamiento de una beta...

**¿Cómo hacemos un milestone?**

-   en la pestaña de creacion de tu issue, a la derecha aparece "milestone"... ahí lo creas
-   dentro de la pestaña "issues"... abajito (al costado de new issue) podras ver una pestañita de **milestones**, ahí aparecerán todos, podras modificarlos... por ejemplo la fecha, cerrarlo o borrarlo, etc.
-   en tu pestaña issues puedes filtrar por milestone
-   a medida que cierras los issues pertenecientes a dicho milestone, el progreso de este se irá actualizando

## Agregando colaboradores a un repositorio

**¿Cómo agregas un colaborador?**
settings > manage access > invite a collaborator

ahora puedes asignar personas a los issues
dicho colaborador puede: clonar repo, crear rama, borrar repo... tiene el control del repo hasta cierto punto.

**por eso debes trabajar con ramas o feature branches**

si quieres transferir la propiedad del repo, eso se hace desde settings > Opttions > Danger Zone > Transfer ownership
