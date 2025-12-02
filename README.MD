# Tarea: Sincronización con Repositorios Remotos

## git fetch, git pull y git rebase

### Anxo Vázquez Lorenzo (1DAM)

## Parte 1

### Paso 1

Una vez listo el repositorio en github con los archivos del ejercicio de `hundir la flota` y clonado localmente, accedo al repositorio de github y 
modifico el archivo `tablero.py`

![tablero](./images/mod_tablero.png)

### Paso 2

Modifico el archivo `barco.py` localmente y realizo un commit

![barco](./images/mod_barco.png)

### Paso 3

Me traigo los cambios para descargar el commit remoto sin fusionar.

![fetch](./images/fetch_p1p3.png)

### Paso 4

```
git log main..origin/main
commit 733cdd937880ac8fa73e419c0b5b687a00cd3471 (origin/main, origin/HEAD)
Author: anxovaz <avazquezlorenzo@danielcastelao.org>
Date:   Tue Dec 2 14:06:18 2025 +0100

    Arreglo tablero.py comillas

commit 9179bfd3e0f9059751da2b3bd5ae3d6900214f61
Author: anxovaz <avazquezlorenzo@danielcastelao.org>
Date:   Tue Dec 2 14:05:39 2025 +0100

    modificacion tablero.py
anxo@fedora:~/dam1/COD/1trim/tarea-actualizacion$ 
```

### Paso 5

Realizo un `git merge`

![merge](./images/merge.png)


## Parte 2

### Paso 6

Accedo a github y modifico el archivo `barco.py`.

![barco](./images/mod_barco_github.png)

### Paso 7

Cambio localmente `tablero.py`:

![cambio-tablero](./images/cambio_tablero_2.png)

Y realizo un `commit` local:

```
git commit -am "Segundo commit local"
```

### Paso 8

Sincronizo con `rebase`.

![pull-rebase](./images/pull_rebase.png) 

## Parte 3

Modifico `tablero.py` en remoto.

![tablero](./images/cambio3_tablero.png)

Hago cambios en `barco.py` y creo un `commit` local.

![barco2](./images/cambios2_barco.png)

Utilizo `fetch` de `pycharm`.

![pc-fetch](./images/pc_fetch.png)

Después uso `merge`

![pc-merge](./images/pc_merge.png)

Para terminar hago un último pull con las actualizaciones del `Readme`