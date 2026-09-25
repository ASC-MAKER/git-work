<center>

# TÍTULO DE LA PRÁCTICA


</center>

***Nombre:***
***Curso:*** 2º de Ciclo Superior de Desarrollo de Aplicaciones Web.

### ÍNDICE

+ [Introducción](#id1)
+ [Objetivos](#id2)
+ [Material empleado](#id3)
+ [Desarrollo](#id4)
+ [Conclusiones](#id5)


#### ***Introducción***. <a name="id1"></a>

Para esta actividad hemos investigado los comandos y las utilizaciones de Git y GitHub, y se utiliza cualquier editor de texto  para los cambios en local y sobre todo la preparación y distribución de trabajo debían estar listos antes de empezar.

#### ***Objetivos***. <a name="id2"></a>

Aprender a utilizar GitHub y Git, manejar el control de errore y trabajar en equipo. 

#### ***Material empleado***. <a name="id3"></a>
- Ratón  
- Teclado  
- Portátil  
- VSCode  
- CMD  
- Git  
- Navegador Web (LibreWolf)  
- GitHub  
#### ***Desarrollo***. <a name="id4"></a>

1.- user1 creará un repositorio público llamado git-work en su cuenta de GitHub, añadiendo un README.md y una licencia MIT.  
Lo creamos a través de la página de GitHub.

2.- user1 clonará el repo y añadirá los ficheros: index.html, bootstrap.min.css y cover.css. Luego subirá los cambios al upstream.  
Clonamos con git clone https://github.com/ASC-MAKER/gitwork.git

3.- user2 creará un fork de git-work desde su cuenta de GitHub.  
Se creó desde la interfaz web de GitHub

4.- user2 clonará su fork del repo.  
Clonado con éxito dede GitHub

5.- user1 creará una issue con el título "Add custom text for startup contents".  
Creado desde GitHub y subido en img, aunque también se podía usar gh pr con GitHub CLI instalado

6.- user2 creará una nueva rama custom-text y modificará el fichero index.html personalizándolo para una supuesta startup.  
Creada desde GitHub web y modificado con el editor de GitHub.

7.- user2 enviará un PR a user1.  
Enviado desde interfaz web

8.- user1 probará el PR de user2 en su máquina (copia local) creando previamente un remoto denominado upstream, y realizará ciertos cambios en su copia local que luego deberá subir al propio PR.  
Se creó y subió con éxito utilizando GitHub

9.- user1 y user2 tendrán una pequeña conversación en la página del PR, donde cada usuario incluirá, al menos, un cambio más.  

10.- user1 finalmente aprobará el PR, cerrará la issue creada (usando una referencia a la misma) y actualizará la rama principal en su copia local.  
Se aprobó con exito y se actualizó la rama en la copia local usando git pull

11.- user2 deberá incorporar los cambios de la rama principal de upstream en su propia rama principal.  

12.- user1 creará una issue con el título "Improve UX with cool colors".  

13.- user1 cambiará la línea 10 de cover.css a: color: purple;  

14.- user1 hará simplemente un commit local en main → NO HACER git push.  

15.- user2 creará una nueva rama cool-colors y cambiará la línea 10 de cover.css a: color: darkgreen;  

16.- user2 enviará un PR a user1.  

17.- user1 probará el PR de user2 (en su copia local). A continuación tratará de mergear el contenido de la rama cool-colors en su rama principal y tendrá que gestionar el conflicto: Dejar el contenido que viene de user2.  
Se mergeó con éxito, no se vio el conflicto a simple vista

18.- Después del commit para arreglar el conflicto, user1 modificará la línea 11 de cover.css a: text-shadow: 2px 2px 8px lightgreen;  
19.- user1 hará un commit especificando en el mensaje de commit el cambio hecho (sombra) y que se cierra la issue creada (usar referencia a la issue). A continuación subirá los cambios a origin/main.  
Aquí se hicieron las comprobaciones para el paso 18 y 19 en la terminal de Git. Se deja el paso a paso sin los resultados de los comandos ejecutados para comprobar y arreglar el estado del repo y sus conflictos. 

adani@LAPTOPASC MINGW64 ~/Desktop/git-work (main)
$ git push origin main

adani@LAPTOPASC MINGW64 ~/Desktop/git-work (main)
$ git pull origin main

adani@LAPTOPASC MINGW64 ~/Desktop/git-work (main|MERGING)
$ git status

adani@LAPTOPASC MINGW64 ~/Desktop/git-work (main|MERGING)
$ git add a1/files/cover.css

adani@LAPTOPASC MINGW64 ~/Desktop/git-work (main|MERGING)
$ git commit -m "Merge branch 'main' of https://github.com/ASC-MAKER/git-work into main"

adani@LAPTOPASC MINGW64 ~/Desktop/git-work (main)
$ git push origin main

adani@LAPTOPASC MINGW64 ~/Desktop/git-work (main)
$ git status

20.- user1 etiquetará esta versión (en su copia local) como 0.1.0 y después de subir los cambios creará una "release" en GitHub apuntando a esta etiqueta.  
git tag -a 0.1.0 -m "Versión 0.1.0"
git push origin 0.1.0

Las dificultades que tuvimos fueron realmete por la falta de entendimiento de pasos como el 9, 10 y 11, porque habían muchas maneras de poder hacerlo y no teníamos clara cual se pedía. Simplemente avanzamos como creímos mejor y seguimos con el resto de pasos.
#### ***Conclusiones***. <a name="id5"></a>

En esta parte debemos exponer las conclusiones que sacamos del desarrollo de la prácica.
