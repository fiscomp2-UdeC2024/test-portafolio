# Portafolio - Física Computacional II (UdeC 510240 - 2023)

Incluya evidencias de programación relacionadas con actividades de su
asignatura. Este producto será evaluado mediante la plataforma
[GitHub](https://github.com). Es su responsabilidad mantener este
repositorio actualizado.

- El documento principal es [portafolio.tex](portafolio.tex).
- Para cada evidencia, deberá crear un documento de latex que será alojado en la carpeta [tex/](tex/), con imágenes en la subcarpeta [img/](img/).
- Si usted crea software (pogramas de python), estas deben estar alojadas en la carpeta [src](src/).


<details>
	<summary> Instrucciones para instalar y configurar Git </summary>

## Cómo instalar Git
Primero, debes instalar Git en tu sistema operativo:
- [Linux](https://git-scm.com/download/linux)
- [Mac](https://git-scm.com/download/mac)
- [Windows](https://git-scm.com/download/win)

## Configurar usuario
Si ves este documento, significa que ya creaste un usuario y
contraseña en [GitHub](https://github.com).

Luego, debes configurar git para poder comunicar tu computador con
GitHub. Para ello, abre la consola de Git en tu computador (o la
terminal en mac/linux) y escribe:

```git
git config --global user.name "Nombre Apellido"
git config --global user.email "usuario@email.com"
```

Por favor, usa tu nombre real en la primera línea.

### Configuración para computadores personales
A continuación, debes crear una [llave SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent). En la misma consola de Git, escribe:

```git
ssh-keygen -t ed25519 -C "usuario@email.com"
```

Esto creará un archivo `id_ed25519.pub` en tu carpeta personal (`~/.ssh/` en linux/mac, `C:\Users\tu_usuario\.ssh` en windows). **Copia el contenido de ese archivo**.

Finalmente, abre la configuración de GitHub y busca "SSH and GPG keys" ([o pincha este link](https://github.com/settings/keys)). A la derecha, verás un botón verde "New SSH key". En `título` escribe un texto descriptivo de la llave (por ejemplo, "mi computador personal"). En `Key`, pega el contenido del archivo `id_ed25519.pub`. Puedes ver más [detalles aquí](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

### Configuración para computadores públicos

Abre la [configuración de tu cuenta](https://github.com/settings/profile) en GitHub.
- Busca [Developer settings](https://github.com/settings/apps).
- Selecciona \texttt{Personal access tokens} y luego [tokens](https://github.com/settings/tokens).
- Aprieta el botón [Generate new token (classic)](https://github.com/settings/tokens/new).
  - En `Note` escribe un comentario que describa para qué es esta clave.
  - Selecciona la feha de expiración (expones tu cuenta si colocas `No expiration`).
  - En `scopes`, selecciona `repo` (que te permitirá tener total control sobre tu repositorio).
  - Al final de la página, aprieta el botón verde `Generate token`.
  - Copia la clave generada (la verás en un cuadro verde) y guárdala en un lugar seguro.
  - No podrás recuperar esta clave. Si la olvidas, debes crear una nueva. 

- Cuando actualices un repositorio (via `git clone`, `git fetch`, `git
pull`, o `git push`, te pedirá tu nombre de usuario y la clave que
creaste en el punto anterior.

</details>

<details>
<summary> Instrucciones para descargar/actualizar este repositorio </summary>

## Cómo descargar este repositorio

Primero, en el botón "Code" (arriba a la derecha), selecciona 
- "SSH" si trabajas desde tu computador personal.
- "HTTPS" si trabajas desde un computador público.

Luego copia el link que aparezca ahí.

En tu computador, crea una carpeta donde guardarás los materiales de tus tareas,
por ejemplo `fiscomp2`. Dentro de esta carpeta, escribe el siguiente comando

```git
git clone URL   # reemplaza URL por el link que copiaste
```
que creará una carpeta (probablemente de nombre `portafolio-autor`) dentro `fiscomp2` y donde se descargarán los contenidos de este repositorio.


## Cómo subir tus respuestas al repositorio

Una vez hayas descargado el repositorio, puedes editar, agregar o eliminar los archivos que quieras normalmente dentro de la carpeta `portafolio-autor`). 

Para preparar los cambios de tu repositorio, escribe esta secuencia de comandos en la consola de git:

```git
git add <archivo1> <archivo2> ...
git commit -m "Un mensaje corto que describa los cambios"
```

Repite esta acción cada vez que edites, elimines o agregues archivos a tu trabajo.

Finalmente, antes de cerrar tu computador, asegurate de subir tus archivos a github con:
```git
git push
```
</details>

# Instrucciones generales de entrega

- Al final de mes, el profesor seleccionará al azar un número indeterminado de repositorios y los revisará para entregar feedback. Si el repositorio no ha sido actualizado, se marcará como inactivo y no seguirá siendo evaluado.

- El profesor es libre de revisar el estado de los repositorios y asignar una nota de avance en cualquier momento.

- El portafolio consistirá una colección de evidencias de programación, donde el estudiante deberá resolver una serie de problemas propuestos en las guías de estudio que serán acordados en clases oportunamente.

- El portafolio se revisará únicamente via github. **Cualquier tarea enviada por otro medio (e.g. e-mail) no será
  revisada**. Es su responsabilidad asegurarse que su trabajo sea
  visible en la plataforma.

- Al final de semestre, se revisará un único documento `portafolio.pdf` que será generado con el archivo [portafolio.tex](portafolio.tex). **NO AGREGUE EL PDF**, este será compilado en el computador del profesor.

  - En la carpeta [img/](img/), suba todas las imágenes que vaya a usar para
  apoyar las evidencias de trabajo. Asegúrese de explicar estas figuras en el archivo que corresponda dentro de la carpeta [tex](tex/).

  - En la carpeta `src`, suba todos los programas (escritos en python) que son necesarios para
  responder a cada problema. **Asegúrese de explicarlos** en donde corresponde en los archivos de la carpeta [tex](tex/). Si no explica sus códigos, no serán revisados.

- Este documento se debe confeccionar de forma individual. No se pueden formar grupos.

- No hay perjuicio de que puedan trabajar con otros compañeros/as
  para apoyarse. Sin embargo, **si sus respuestas son idénticas
  o muy similares a las de otros grupos, el profesor es libre de
  calificar con la nota mínima**. El plagio es sancionado por el
  reglamento de la Universidad.

  En caso de plagio entre estudiantes, el profesor considerará como autor original a aquel que haya subido primero sus archivos a la plataforma.

- **Cada** falta ortográfica, ecuación rayada y uso de símbolos no
  justificados (como `$\blacksquare$`, `$\square$`, `q.e.d.`,
  `$\Rightarrow$`, `$\forall$`, `$\exists$`, `$\bot$`, entre otros),
  serán penalizados según rúbricas que se entregarán oportunamente.

- Siéntase libre de eliminar los archivos que no necesite para la confección de su portafolio, pero debe tener cuidado de mantener la configuración de este.

---
Este es un documento escrito en el formato [Markdown de
GitHub](https://guides.github.com/features/mastering-markdown/).
