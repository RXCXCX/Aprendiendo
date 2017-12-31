# Inicio rápido con GIT

```
git init
```

Inicia una seción GIT

```
git status
```
Muestra los cambios hechos agregados y no agregados al stage

```
git add [<-A>, <"namefile">, <'*.extensión'>]
```

Agrega el archivo especificado al stage

-A agrega todos

```
git commit -m "descripción de los cambios"
```

Agrega una entrada al log

```
git log
```

Muestra los commits

```
git checkout [<SHA code>, <branch>]
```

Modifica el estado del área de trabajo hasta el log del SHA code. 

Cambia la rama

```
git reset [<--soft>, <--mixed>, <--HARD>]
```

--soft: elimina los logs hasta donde está el checkout sin modificar el área de trabajo (no modifica el código)

--mixed: elimina los logs sin alterar el área de trabajo hasta el checkout

--HARD: elimina los logs y los cabios hechos hasta el  el checkout en turno

```
git log > ruta.nombre.txt
```

Crea un fichero en ruta.nombre con los logs hasta el checkout en uso

```
git branch
```

muestra las ramas

```
git branch "nombre"
```

crea una nueva rama

```
git branch -D "nombre"
```

Elimina una rama 

```
git merge "rama a absorver"
```

Se fusionan los cambios producidos en la "rama por absorver" en la rama en la que se esté actualmente

## GitHub

```
git clone "HTTPS"
```

Copia los archivos de la repo al directorio actual

```
git remote [<add origin "HTTPS">, <-v>, <remove origin>]
```

add origin "HTTPS": vincula el directorio actual con el origen HTTPS

-v: visualiza el origen actual

remove origin: borra el origen establecido

```
git push origin "branch"
```

Clona el directorio en la rama branch al orígen establecido  