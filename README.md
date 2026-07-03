
# 🚀 GIT Y GITHUB 

## 1. Configuración

| Comando                                             | ¿Para qué sirve?                                         |
| --------------------------------------------------- | -------------------------------------------------------- |
| `git config --global user.name "Tu Nombre"`         | Configura el nombre del autor de los commits.            |
| `git config --global user.email "correo@email.com"` | Configura el correo del autor de los commits.            |
| `git config --global core.editor "code --wait"`     | Configura Visual Studio Code como editor predeterminado. |
| `git config --list`                                 | Muestra toda la configuración de Git.                    |
| `git version`                                       | Muestra la versión instalada de Git.                     |

## 2. Crear o descargar un repositorio

| Comando         | ¿Para qué sirve?                                    |
| --------------- | --------------------------------------------------- |
| `git init`      | Crea un nuevo repositorio Git en la carpeta actual. |
| `git clone URL` | Descarga un repositorio remoto (GitHub).            |

## 3. Estado del proyecto

| Comando             | ¿Para qué sirve?                                       |
| ------------------- | ------------------------------------------------------ |
| `git status`        | Muestra el estado actual del proyecto.                 |
| `git diff`          | Muestra los cambios aún no preparados.                 |
| `git diff --staged` | Muestra los cambios preparados para el próximo commit. |

## 4. Agregar archivos (Staging)

| Comando                        | ¿Para qué sirve?                                               |
| ------------------------------ | -------------------------------------------------------------- |
| `git add archivo`              | Agrega un archivo específico al área de preparación (Staging). |
| `git add .`                    | Agrega todos los cambios al Staging.                           |
| `git restore --staged archivo` | Quita un archivo del Staging sin borrar sus cambios.           |

## 5. Commits

| Comando                    | ¿Para qué sirve?                                        |
| -------------------------- | ------------------------------------------------------- |
| `git commit -m "Mensaje"`  | Guarda los cambios en el historial del proyecto.        |
| `git commit -am "Mensaje"` | Agrega y guarda automáticamente archivos ya rastreados. |
| `git commit --amend`       | Modifica el último commit.                              |

## 6. Historial

| Comando                           | ¿Para qué sirve?                                 |
| --------------------------------- | ------------------------------------------------ |
| `git log`                         | Muestra el historial completo de commits.        |
| `git log --oneline`               | Muestra el historial resumido.                   |
| `git log --graph --oneline --all` | Muestra el historial como un árbol de ramas.     |
| `git show`                        | Muestra la información de un commit.             |
| `git reflog`                      | Muestra todos los movimientos realizados en Git. |

## 7. Ramas (Branches)

| Comando                      | ¿Para qué sirve?                                    |
| ---------------------------- | --------------------------------------------------- |
| `git branch`                 | Lista todas las ramas.                              |
| `git branch nombre-rama`     | Crea una nueva rama.                                |
| `git branch -d nombre-rama`  | Elimina una rama fusionada.                         |
| `git branch -D nombre-rama`  | Fuerza la eliminación de una rama.                  |
| `git switch nombre-rama`     | Cambia a otra rama (recomendado).                   |
| `git switch -c nueva-rama`   | Crea una rama y cambia a ella.                      |
| `git checkout nombre-rama`   | Cambia de rama (comando clásico).                   |
| `git checkout -b nueva-rama` | Crea una rama y cambia a ella (clásico).            |
| `git merge rama`             | Fusiona una rama con la rama actual.                |
| `git rebase rama`            | Reorganiza el historial de commits sobre otra rama. |

## 8. Repositorio remoto (GitHub)

| Comando                         | ¿Para qué sirve?                               |
| ------------------------------- | ---------------------------------------------- |
| `git remote add origin URL`     | Conecta el proyecto local con GitHub.          |
| `git remote -v`                 | Muestra los repositorios remotos configurados. |
| `git remote remove origin`      | Elimina un repositorio remoto.                 |
| `git remote set-url origin URL` | Cambia la URL del repositorio remoto.          |

## 9. Sincronización con GitHub

| Comando                       | ¿Para qué sirve?                               |
| ----------------------------- | ---------------------------------------------- |
| `git fetch`                   | Descarga cambios sin aplicarlos.               |
| `git pull`                    | Descarga y fusiona los cambios.                |
| `git pull --rebase`           | Descarga cambios usando Rebase.                |
| `git pull --merge`            | Descarga cambios usando Merge.                 |
| `git push`                    | Sube los commits al repositorio remoto.        |
| `git push origin rama`        | Sube una rama específica.                      |
| `git push -u origin rama`     | Sube una rama y la vincula al remoto.          |
| `git push --force`            | Fuerza el envío de cambios (usar con cuidado). |
| `git push --force-with-lease` | Fuerza el envío de forma más segura.           |

## 10. Deshacer cambios

| Comando                    | ¿Para qué sirve?                                    |
| -------------------------- | --------------------------------------------------- |
| `git restore archivo`      | Descarta los cambios de un archivo.                 |
| `git restore .`            | Descarta todos los cambios locales.                 |
| `git reset HEAD archivo`   | Quita un archivo del Staging.                       |
| `git reset --soft HEAD~1`  | Deshace el último commit conservando el Staging.    |
| `git reset --mixed HEAD~1` | Deshace el commit dejando los cambios sin preparar. |
| `git reset --hard HEAD~1`  | Elimina el commit y los cambios (⚠️ irreversible).  |
| `git revert HASH`          | Crea un nuevo commit que deshace otro commit.       |

## 11. Stash (Guardar trabajo temporal)

| Comando           | ¿Para qué sirve?                    |
| ----------------- | ----------------------------------- |
| `git stash`       | Guarda cambios temporalmente.       |
| `git stash list`  | Lista los Stash guardados.          |
| `git stash pop`   | Recupera y elimina el último Stash. |
| `git stash apply` | Recupera un Stash sin eliminarlo.   |
| `git stash drop`  | Elimina un Stash específico.        |
| `git stash clear` | Elimina todos los Stash.            |

## 12. Etiquetas (Tags)

| Comando                        | ¿Para qué sirve?                   |
| ------------------------------ | ---------------------------------- |
| `git tag`                      | Lista las etiquetas.               |
| `git tag v1.0`                 | Crea una etiqueta.                 |
| `git tag -a v1.0 -m "Versión"` | Crea una etiqueta con descripción. |
| `git push origin v1.0`         | Sube una etiqueta al remoto.       |
| `git push --tags`              | Sube todas las etiquetas.          |
| `git tag -d v1.0`              | Elimina una etiqueta local.        |

## 13. Otros comandos útiles

| Comando                                   | ¿Para qué sirve?                                |
| ----------------------------------------- | ----------------------------------------------- |
| `git clean -f`                            | Elimina archivos no rastreados.                 |
| `git clean -fd`                           | Elimina archivos y carpetas no rastreados.      |
| `git clean -fdx`                          | Elimina incluso archivos ignorados.             |
| `git blame archivo`                       | Muestra quién modificó cada línea.              |
| `git cherry-pick HASH`                    | Copia un commit específico a la rama actual.    |
| `git bisect start`                        | Inicia la búsqueda del commit con un error.     |
| `git bisect good`                         | Marca un commit como correcto.                  |
| `git bisect bad`                          | Marca un commit como incorrecto.                |
| `git bisect reset`                        | Finaliza la búsqueda con Bisect.                |
| `git ls-files`                            | Lista los archivos rastreados por Git.          |
| `git check-ignore -v archivo`             | Indica por qué un archivo está siendo ignorado. |
| `git submodule add URL`                   | Agrega un submódulo al proyecto.                |
| `git submodule update --init --recursive` | Descarga e inicializa los submódulos.           |
| `git help`                                | Muestra la ayuda general de Git.                |
| `git help comando`                        | Muestra la ayuda de un comando específico.      |

## Flujo de trabajo básico

`git clone URL` → `git status` → `git add .` → `git commit -m "Mensaje"` → `git pull` → `git push`

## Comandos imprescindibles

`git init` • `git clone` • `git status` • `git add .` • `git commit -m` • `git push` • `git pull` • `git fetch` • `git branch` • `git switch` • `git merge` • `git log --oneline` • `git diff` • `git stash` • `git restore` • `git reset` • `git revert` • `git remote -v`
