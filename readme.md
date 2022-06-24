#Practica 1

## Ejercicio 1

**¿Qué comando utilizaste en el paso 11? ¿Por qué?**

Git reset --hard HEAD~1 porque permite mover el puntero sobre el que esté situado HEAD hacia el commit  anterior sin guardar los cambios del working area.

**¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**

Git reset --hard <hash>, así podía revertir al identificador del commit y recuperar el contenido del working area en el proceso.

**El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**

No, porque la rama styled ya contenía todos los cambios que se habían hecho previamente sobre la rama main y en este caso el merge fue fast-forward.

**El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**

Sí, porque había varios cambios que afectaban a las mismas partes del código de ambas ramas y por esto hubo que seleccionar los cambios que queríamos preservar y el merge no pudo ser fast-forward.

**El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**

No, tampoco hubo conflictos. En este caso el merge se produjo fast-forward sin inconvenientes.

**¿Qué comando o comandos utilizaste en el paso 25?**

Usé git log --graph para poder ver una representación del grafo en consola.

**El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**

Si, podría ser perfectamente fast-forward porque la rama master contiene todo el trabajo de la rama title y unicamente se añade una pequeña modificación al texto.

**¿Qué comando o comandos utilizaste en el paso 27?**

Un git reset HEAD~1 para desplazarme al estado anterior al merge pero preservando los cambios en el working area.

**¿Qué comando o comandos utilizaste en el paso 28?**

Un git restore git-nuestro.md para eliminar el archivo modificado del working area.

**¿Qué comando o comandos utilizaste en el paso 29?**

git branch -D title, para forzar el borrado

**¿Qué comando o comandos utilizaste en el paso 30?**

git reset --hard <hash>

**¿Qué comando o comandos usaste en el paso 32?**

Git reflog para localizar el hash y luego git reset <hash> para desplazarme hasta el commit inicial.

**¿Qué comando o comandos usaste en el punto 33?**

Use un git reflog para saber el <hash> y luego un git reset <hash> para volver al estado final.