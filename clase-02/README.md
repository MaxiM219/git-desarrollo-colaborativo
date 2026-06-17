# Clase 02 - Git Desarrollo Colaborativo

## Forma corta de vvisualizar el status

```sh
git status --short
```

## Ramas (Branches)

```sh
git branch
```

## Crear rama

```sh
git branch <nombre-rama>
git branch feature/branches
```

## Cambiar de rama

```sh
git switch <nombre-rama>
git switch feature/branches
git switch - # Moverse entre las últimas ramas que estuvimos
```

## Borrar una rama

```sh
git branch -d <nombre-rama>
git branch -d feature/branches
```

## Creamos y nos movemos a la rama

```sh
git switch -c <nombre-rama>
git switch -c feature/branches
```

## Ver diferencias entre ramas

```sh
git diff feature/branches # Estando en main
git diff main # Estando en feature/branches
```

# Fusiones entre ramas

## 3 formas que git va a realizar la fusión

* Fast-forward -> Git resuelve por nosotros todo. Lo hace automaticamente
* Triple via -> Git resuelve por nosotros todo. Lo hace automaticamente.
* Conflicto -> Git no puede saber que cambios son los que quiero dejar y entra en conflicto. Manualmente. El desarrollo o desarrollodores tienen que ayudar a git a resolver el conflicto.

# Herramientas visulaes para trabajar con GIT

* Github Desktop -> 
* gitkraken -> 

# Subir al repo remoto el repo local
Subir a Github un repositorio local es tener una copia exacta (copia espejo) sincronizada del repo local en un remoto.

> Agregar a mi repo local la ruta o dirección al

```sh
git remote add <alias> <url-al-remoto>
git remote add origin ...
```

> Enviar los cambios al remoto

```sh
git push -u <alias-remoto> <rama-local>
git push -u origin main # indica a git que automaticamente la proxima vez que haga push se haga a la rama main remota.
git push # segunda y siguientes veces y automaticamente se sube la rama local main a la rama remota main
```

## Traernos los cambios del remoto

### Git Pull
Nos trae la meta data que se encuentra en la carpeta .git. No trae los cambios, solo la meta data.
Actualiza la carpeta .git

```sh
git fetch
```

### Git Pull 
Traer la metadata y cambios

```sh
git fetch
```

## Ver ramas locales y remotas
Veo las ramas, su estado y en que commit quedaron esas ramas

```sh
git branch -r
```

