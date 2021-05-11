# ![alt text](https://assets.breatheco.de/apis/img/images.php?blob&random&cat=icon&tags=breathecode,32) API estática del árbol genealógico

Basado en las tecnologías/estrategias que hemos aprendido, construye una API estática que maneje un árbol familiar. Tu eres libre de usar tu propia información familiar, también puedes usar datos falsos.

## 🌱  Cómo iniciar este proyecto

 No clones este repositorio. El primer paso para comenzar a codificar es clonar el [python boilerplate](https://github.com/4GeeksAcademy/flask-rest-hello) en tu compjutador local o con Gitpod.

a) Si usas Gitpod (recomendada) puedes clonar el boilerplate [clic aquí](https://github.com/4GeeksAcademy/flask-rest-hello).

b) Si trabajas localmente, escribe el siguiente comando en tu terminal: 
```sh
git clone  git clone https://github.com/4GeeksAcademy/flask-rest-hello
```
💡 Important: Remember to create a new repository, update the remote (`git remote set-url origin <your new url>`), and upload the code to your new repository using `add`, `commit` and `push`.

## :memo: Instrucciones

Tu API debe tener, al menos, 7 miembros distribuidos en 3 generaciones: 

**abuelos -> padres -> generación actual**

El árbol genealógico debe representarse como un árbol de objetos estructurados, es decir: cada persona (nodo en el árbol) debe tener: id, nombre, apellido, edad y una referencia (id) a sus padres e hijos (si corresponde).

- `GET /all`: La API debe exponer un endpoint que devuelva la lista completa de miembros de la familia ordenados por mayor a menor.

- `GET /member/<int:id>`: La API debe exponer un endpoint que devuelve a un miembro específico del árbol familiar por su id (que debe ser único) y la información sobre sus hijos y padres.

### Tecnologías

La API se debe desarrollar utilizando **Flask** y cada punto final debe devolver un archivo *válido* **JSON**.

### Pista

Es posible que desees dibujar (lápiz y papel) la estructura de árbol para tener una estructura "visual" en mente. Usa las líneas para mostrar las referencias entre padres e hijos.

Las referencias deben ser el número de identificación de los miembros.

Crea tus estructuras de datos antes de crear los puntos finales o endpoints, use variables globales.
