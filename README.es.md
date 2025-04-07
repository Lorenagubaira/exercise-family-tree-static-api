<!--hide-->
# API estática del árbol genealógico
<!--endhide-->

Basado en las tecnologías/estrategias que hemos aprendido, construye una API estática que maneje un árbol familiar. Tú eres libre de usar tu propia información familiar, también puedes usar datos falsos.

<how-to-start>

## 🌱 Cómo iniciar este proyecto

No clones este repositorio porque usaremos una plantilla diferente.  

Recomendamos abrir el `python boilerplate` ó  `nodejs boilerplate`, utilizando una herramienta de aprovisionamiento como [Codespaces](https://4geeks.com/lesson/what-is-github-codespaces) (recomendado) o [Gitpod](https://4geeks.com/lesson/how-to-use-gitpod). Alternativamente, puedes [clonar el repositorio de GitHub](https://4geeks.com/how-to/github-clone-repository) en tu computadora local utilizando el comando `git clone`.  

Estos son los repositorios que puedes abrir o clonar:  

- Python:
```sh
$ git clone https://github.com/4GeeksAcademy/flask-rest-hello
```
- Nodejs:
```sh
$ git clone https://github.com/4GeeksAcademy/expressjs-rest-hello
```

💡 Importante: Recuerda crear un nuevo repositorio, actualizar el remoto (`git remote set-url origin <tu nueva url>`), y subir el código a tu nuevo repositorio utilizando `add`, `commit` y `push`.  

</how-to-start>

## :memo: Instrucciones

Tu API debe tener, al menos, 7 miembros distribuidos en 3 generaciones: 

**abuelos -> padres -> generación actual**

El árbol genealógico debe representarse como un árbol de objetos estructurados, es decir: cada persona (nodo en el árbol) debe tener: id, nombre, apellido, edad y una referencia (id) a sus padres e hijos (si corresponde).

- `GET /all`: La API debe exponer un endpoint que devuelva la lista completa de miembros de la familia ordenados por mayor a menor.

- `GET /member/<int:id>`: La API debe exponer un endpoint que devuelve a un miembro específico del árbol familiar por su id (que debe ser único) y la información sobre sus hijos y padres.

### Tecnologías

La API se debe desarrollar utilizando **Flask** or **Expressjs** y cada punto final debe devolver un archivo *válido* **JSON**.

### Pista

Es posible que desees dibujar (lápiz y papel) la estructura de árbol para tener una estructura "visual" en mente. Usa las líneas para mostrar las referencias entre padres e hijos.

Las referencias deben ser el número de identificación de los miembros.

Crea tus estructuras de datos antes de crear los puntos finales o endpoints, use variables globales.
