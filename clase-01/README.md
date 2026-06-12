# Clase 01 - Git Desarrollo Colaborativo

## Verificar que se haya instalado GIT

```
git --version
```

## Ver estado y área en la que están mis archivos

```
git status
```

## Los archivos pueden estar en varios estados dentro del proyecto

* untracked -> El archivo existe, git sabe que existe pero no le está dando seguimiento.
* modified -> Los cambios dentro del archivo difieren de los cambios del archivo en el repositorio local
* staged -> Los cambios dentro del archivo están confirmados para ser un commit

## Ver historial de commits (Historia del repositorio)

```sh
git log # larga
git log --oneline #corta
```

## Comparar estado de los archivos. Entre WD y LR

```sh
git diff
```

## Comparar estado de los archivos. Entre WD y SA | SA y LR

```sh
git diff --staged # Que depende donde están las modificaciones es la referencia
```