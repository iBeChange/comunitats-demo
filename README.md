# Comunitats · demo interactiva

Prototipo navegable de la nueva sección de Comunitat: pantalla principal, categorías con hilos, filtros por etiqueta y etapa, hilo abierto con respuestas y creación de un hilo nuevo.

Es una demo para enseñar al equipo. Todos los nombres, mensajes y cifras son ejemplos inventados, y los textos entre corchetes (`[DATA]`, `[LLOC]`…) son marcadores para sustituir.

## Qué se puede probar

- **Pantalla Comunitat**: buscador, chips de “El meu moment” (cambian los hilos de “Ara a la comunitat”), Plafó con sus tres ventanas (Tallers i activitats, Actualitat y Recursos), acceso a la Benvinguda y los cinco bloques.
- **Bloque con filtros**: al entrar en un bloque aparecen todos sus hilos. Arriba, las subcategorías como chips, debajo las etiquetas y, por último, el orden (recientes, más activos, sin respuesta) y la etapa. Cada hilo indica su subcategoría. Los hilos fijados del equipo salen primero y hay un elemento del Plafó intercalado.
- **Etiquetas cruzadas**: un hilo vive en una categoría, pero aparece también en otras por sus etiquetas. Por ejemplo, el hilo de insomnio está en *Hormonoteràpia i efectes* y sale también en *Descans i son*, marcado como “Des de…”.
- **Hilo abierto**: reacciones “M’hi identifico”, respuestas con la etapa de cada persona y un interruptor para destacar las respuestas de tu mismo momento. Se puede responder.
- **Nou fil**: elegir categoría, escribir, recibir etiquetas sugeridas según el texto (máximo dos, de una lista cerrada), confirmar o cambiar la etapa y decidir si se muestra.
- **Barra inferior**: Perfil, Comunitat y Missatges.
- **Perfil**: nombre, etapa, visibilidad, hilos guardados y propios, y un botón para restablecer la demo.

Lo que se crea se guarda solo en el navegador de cada persona (localStorage). No hay servidor ni base de datos.

## Verla en local

Abre `index.html` con doble clic. Es un único archivo que lo contiene todo, así que funciona por sí solo.

## Publicarla con GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo, `comunitats-demo`).
2. Sube `index.html` y este `README.md` con **Add file → Upload files**.
3. Ve a **Settings → Pages**. En *Source* elige **Deploy from a branch**, la rama `main` y la carpeta `/ (root)`. Guarda.
4. En uno o dos minutos GitHub mostrará el enlace, del tipo `https://<usuario>.github.io/comunitats-demo/`.

## Editar el contenido

Todo está dentro de `index.html`: primero los estilos, después los datos de ejemplo (bloques, categorías, etiquetas, etapas, Plafó e hilos) y al final la lógica de la app. Cada etiqueta tiene una lista de palabras clave (`keys`) que se usa para sugerirla al escribir un hilo.
