# FAQs Wiki

En esta sección encontrarás las preguntas más frecuentes sobre el uso de la wiki.

<details>
<summary>**1. ¿Cómo subo una nueva página?**</summary>

1. Ubicar la carpeta “docs” dentro del repositorio.
2. Dentro de la carpeta “docs”, ubicar la carpeta en la cual queremos añadir una página.
3. Una vez dentro de dicha carpeta, dar click a “add files” ubicado arriba a la derecha.
4. El nombre del archivo debe ser definido de la siguiente manera: **nombre-de-página.md**.
5. Recuerda agregar el .md
6. Escribe tu página en MarkDown.
7. Cuando hayas finalizado, da click a “commit changes” ubicado arriba a la derecha.
8. Espera 1 minuta para que tu cambio se vea reflejado en la página.
</details>

<details>
<summary>**2. ¿Cómo subo una nueva carpeta?**</summary>

1. Ubicar la carpeta “docs” dentro del repositorio.
2. Dentro de la carpeta “docs”, dar click a “add files” ubicado arriba a la derecha.
3. El nombre de la carpeta debe ser definido de la siguiente manera: **nombre-de-carpeta/nombre-de-página.md**.
4. El primer nombre hace referencia a cómo se llamará la carpeta mientras que el nombre después del “/“ se refiere al nombre de una página dentro de la nueva carpeta.
5. Agrega un archivo _category_.json. Este archivo contiene información para la configuración de la carpeta.
6. Cuando hayas finalizado, da click a “commit changes” ubicado arriba a la derecha.

```
{
  "label": “Nombre de la carpeta”,
  "position": num,  //posición de la carpeta en la lista (asegúrate de no escribir un número ya existente)
  "link": {
    "type": "generated-index"
  }
}
```

</details>

<details>
<summary>**3. Me marca error cuando uso `<br>` ¿qué hago?**</summary>

Si estamos utilizando lo siguiente:
`<br>`
Es necesario especificar que es una etiqueta de cierre, por lo que debe de quedar así:
`<br />`

</details>

<details>
<summary>**4. No se suben mis cambios ¿qué hago?**</summary>

Puedes verificar el estatus de tu código en la sección de “**Actions**” que se encuentra al lado del botón “Pull Request”, ahí podrás identificar si tus cambios están en proceso, si ya se desplegaron o si los cambios fueron rechazados por un error.

</details>

<details>
<summary>**5. ¿Cómo cambio el orden el que aparecen las páginas en la barra lateral?**</summary>

Para esto tienes que agregar una sección de metadata al inicio del archivo .md de la siguiente manera:

```
---
sidebar_position: 1
---

...resto del contenido...
```

- Los 3 guiones al inicio y al final son necesarios para que el archivo sea reconocido como una página de documentación.
- El número que se encuentra después de `sidebar_position` indica la posición en la que aparecerá la página en la barra lateral. Mientras más pequeño sea el número, más arriba aparecerá la página.

**Procura que no existan dos páginas con el mismo sidebar_position dentro de una sección**.

</details>
