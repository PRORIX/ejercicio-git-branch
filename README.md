# Comenzando a trabajar con branch
## Romén Gilberto García Gómez

### Creamos un nuevo branch en el repositorio que ya hemos clonado

```bash
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git checkout -b ejercicio1-branch
Cambiado a nueva rama 'ejercicio1-branch'
```

### Añadimos una nueva clase al repositorio

```bash
public class Ejercicio1 {
    public static void main (String[] args) {
        System.out.println("Ejercicio 1 realizado.");
    }
}
```

###  Hacemos un commit de los cambios

```bash
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git add .
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git commit -m "se incluye el Ejercicio1.java"
[ejercicio1-branch cfad067] se incluye el Ejercicio1.java
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Ejercicio1.java
```

### Subimos la rama nueva con los cambios al repositorio remoto

```bash
 git push --set-upstream origin ejercicio1-branch
Enumerando objetos: 4, listo.
Contando objetos: 100% (4/4), listo.
Compresión delta usando hasta 4 hilos
Comprimiendo objetos: 100% (2/2), listo.
Escribiendo objetos: 100% (3/3), 304 bytes | 304.00 KiB/s, listo.
Total 3 (delta 0), reusados 0 (delta 0), pack-reusados 0
remote: 
remote: Create a pull request for 'ejercicio1-branch' on GitHub by visiting:
remote:      https://github.com/PRORIX/ejercicio-git-branch/pull/new/ejercicio1-branch
remote: 
To https://github.com/PRORIX/ejercicio-git-branch
 * [new branch]      ejercicio1-branch -> ejercicio1-branch
Rama 'ejercicio1-branch' configurada para hacer seguimiento a la rama remota 'ejercicio1-branch' de 'origin'.
```

### Fusionamos la rama en main y la subimos a GitHub

```bash
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git checkout main
Cambiado a rama 'main'
Tu rama está actualizada con 'origin/main'.
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git merge ejercicio1-branch
Actualizando 5df4ac1..cfad067
Fast-forward
 Ejercicio1.java | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Ejercicio1.java
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git push
Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
To https://github.com/PRORIX/ejercicio-git-branch
   5df4ac1..cfad067  main -> main
```

### Repetimos todos los pasos con el Ejercicio 2

```bash
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git checkout -b ejercicio2-branch
Cambiado a nueva rama 'ejercicio2-branch'
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git add .
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git commit -m
error: switch `m' requiere un valor
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git commit -m "se incluye el Ejercicio2.java"
[ejercicio2-branch 7a2ce9f] se incluye el Ejercicio2.java
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Ejercicio2.java
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git push --set-upstream origin ejercicio2-branch
Enumerando objetos: 3, listo.
Contando objetos: 100% (3/3), listo.
Compresión delta usando hasta 4 hilos
Comprimiendo objetos: 100% (2/2), listo.
Escribiendo objetos: 100% (2/2), 299 bytes | 299.00 KiB/s, listo.
Total 2 (delta 0), reusados 0 (delta 0), pack-reusados 0
remote: 
remote: Create a pull request for 'ejercicio2-branch' on GitHub by visiting:
remote:      https://github.com/PRORIX/ejercicio-git-branch/pull/new/ejercicio2-branch
remote: 
To https://github.com/PRORIX/ejercicio-git-branch
 * [new branch]      ejercicio2-branch -> ejercicio2-branch
Rama 'ejercicio2-branch' configurada para hacer seguimiento a la rama remota 'ejercicio2-branch' de 'origin'.
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git checkout main
Cambiado a rama 'main'
Tu rama está actualizada con 'origin/main'.
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git merge ejercicio2-branch
Actualizando cfad067..7a2ce9f
Fast-forward
 Ejercicio2.java | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Ejercicio2.java
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git push
Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
To https://github.com/PRORIX/ejercicio-git-branch
   cfad067..7a2ce9f  main -> main
```

### Repetimos todos los pasos con el Ejercicio 3

```bash
:~/ejercicio-git-branch$ git checkout -b ejercicio3-branch
Cambiado a nueva rama 'ejercicio3-branch'
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git add .
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git commit -m "se incluye el Ejercicio3.java
> "
[ejercicio3-branch 33d66d2] se incluye el Ejercicio3.java
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Ejercicio3.java
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git push --set-upstream origin ejercicio3-branch
Enumerando objetos: 3, listo.
Contando objetos: 100% (3/3), listo.
Compresión delta usando hasta 4 hilos
Comprimiendo objetos: 100% (2/2), listo.
Escribiendo objetos: 100% (2/2), 259 bytes | 259.00 KiB/s, listo.
Total 2 (delta 1), reusados 0 (delta 0), pack-reusados 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ejercicio3-branch' on GitHub by visiting:
remote:      https://github.com/PRORIX/ejercicio-git-branch/pull/new/ejercicio3-branch
remote: 
To https://github.com/PRORIX/ejercicio-git-branch
 * [new branch]      ejercicio3-branch -> ejercicio3-branch
Rama 'ejercicio3-branch' configurada para hacer seguimiento a la rama remota 'ejercicio3-branch' de 'origin'.
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git checkout main
Cambiado a rama 'main'
Tu rama está actualizada con 'origin/main'.
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git merge ejercicio3-branch
Actualizando 7a2ce9f..33d66d2
Fast-forward
 Ejercicio3.java | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 Ejercicio3.java
bae2@jpexposito-VirtualBox:~/ejercicio-git-branch$ git push
Total 0 (delta 0), reusados 0 (delta 0), pack-reusados 0
To https://github.com/PRORIX/ejercicio-git-branch
   7a2ce9f..33d66d2  main -> main
```
