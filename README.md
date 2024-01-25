# En Español
## Pares de traducciones Español-Extremeño

Este repositorio almacena pares de frases y palabras en Español y Extremeño línea a línea en diferentes ficheros por idioma para entrenar modelos de traducción que puedan ser usados en traductores como por ejemplo [LibreTranslate](https://libretranslate.com/).


## Contribuir
Si quieres contribuir a la recopilación de datos, puedes editar los ficheros añadiendo las partes nuevas y crear un Pull Request para añadirlo al repositorio. Si no sabes como crear PR, puedes crear una petición en [este enlace](https://github.com/juanro49/recursos_es-ext/issues) adjuntando los ficheros actualizados para que los actualicemos en el repositorio tras una revisión de que las palabras son correctas. Si no sabes hacer las dos anteriores o no tienes cuenta en Github, puedes enviarme los textos al email [juanro49+canteaol@disroot.org](mailto:juanro49+canteaol@disroot.org).

Es recomendable que si un párrafo tiene varias frases que tienen sentido por si solas, cada frase vaya en una línea en lugar de una línea con el párrafo completo. En el caso de palabras, es recomendable (si disponen de ellas), añadir sus formas masculinas, femeninas, singular y plural. Si son verbos, se recomienda añadir a conjugación completa.

Estos recursos sirven para la traducción de Español a Extremeño, pero también podría usarse para traducir de Extremeño a Español. El problema es que [Stanza](https://github.com/stanfordnlp/stanza), una dependencia que usa [argos-train](https://github.com/argosopentech/argos-train) para crear los modelos de traducción, no tiene modelos de la lengua extremeña, o que dificulta la traducción en ese sentido y sea mucho menos precisa. Si eres lingüista o tienes experiencia en la creación de vectores de palabras, tokenización de éstas y quieres colaborar en esa parte, puedes echar un vistazo a la [guía sobre como añadir nuevas lenguas](https://stanfordnlp.github.io/stanza/new_language.html).

Si tienes cuenta en github, es recomendable un voto positivo en [este comentario](https://github.com/argosopentech/argos-translate/discussions/91#discussioncomment-1953141) donde tenemos hecha la solicitud para añadir el extremeño a argos-translate y donde iremos adjuntando los modelos que consigamos funcionales para que los añadan a su base de datos y estén disponibles en [LibreTranslate](https://libretranslate.com/).

También tenemos creada [una sección en la comunidad de LibreTranslate](https://community.libretranslate.com/t/github-project-to-collect-extremaduran-spanish-data/516) donde se pueden debatir cosas e iremos poniendo los diferentes modelos que se vayan creando.

### Entrenar modelos
Para el entrenamiento, se puede usar [Argos Train](https://github.com/argosopentech/argos-train) (instrucciones en el enlace).
Para ello necesitamos una gráfica Nvidia compatible con [CUDA](https://developer.nvidia.com/cuda-zone), o una gráfica AMD compatible con [Rocm](https://docs.amd.com/) (Para ésta ultima, es necesario en la instalación reemplazar la versión de pytorch por la [versión que integra Rocm](https://pytorch.org/get-started/locally/)). También es posible usando CPU, pero es mucho mas lento.

En caso de no disponer de una gráfica compatible, se puede optar por un sistema cloud, en mi caso he optado por [Vast.ai](https://cloud.vast.ai/?ref_id=57538) usando la imagen docker de [argos-train](https://hub.docker.com/r/argosopentech/argostrain/tags) que es bastante económico.

Para el entrenamiento, habrá que unir todos los ficheros de cada idioma en uno (importante que se mantenga el orden de los contenidos linea a línea) o usar los denominados contenido-completo, los cuales tienen el contenido de todos los ficheros ya unidos. Para ello se puede usar alguna de las muchas opciones disponibles, como por ejemplo [FilesMerge](https://www.filesmerge.com/sp/merge-text-files) para Windows o el comando `cat` en Gnu/Linux.


## Agradecimientos
Este proyecto surgió por la idea de [Wikimedia España](https://ext.wikipedia.org/wiki/Hundaci%C3%B3n_Wikimedia) de reactivar e impulsar la [Güiquipedia](https://ext.wikipedia.org/), edición de la Wikipedia en la lengua extremeña.

Los recursos de traducción son proporcionados por:
- Contribuciones de voluntarios, especialmente socios de [OscecEstremaura](https://oscecestremaura.wordpress.com/)
- Cadenas de traducciones de [FeedTV](https://github.com/juanro49/FeedTV) (Traducción realizada por [OscecEstremaura](https://oscecestremaura.wordpress.com/)) --> [https://hosted.weblate.org/projects/feedtv/feedtv/ext/](https://hosted.weblate.org/projects/feedtv/feedtv/ext/)
- [El cantón estremeñu](https://elcanton.org/)
- [Dizionariu Estremeñu](https://letterly.github.io/Dizionariu.html)
- [Extremeñistas](https://extremenistas.org/manifiesto-fundacional/)
- [Pedro Moreno](https://moreno-linares.com/)
- [Federación Extremeña de Folklore](https://www.folkloredeextremadura.com/)
- [Wikipedia](https://ext.wikipedia.org/)

Esto es un trabajo comunitario con el único propósito de avanzar culturalmente, en este caso promocionando la lengua extremeña y creando herramientas para facilitar su conocimiento. Por ello, todo el contenido aquí publicado se encontrará bajo licencia [CC0 1.0 de Dominio Público](https://creativecommons.org/publicdomain/zero/1.0/deed.es) para que cualquiera pueda usarlo para crear herramientas o cualquier cosa que sirva para extender y ayudar al conocimiento de la lengua extremeña.

[<img src="https://contrib.rocks/image?repo=juanro49/recursos_es-ext" />](https://github.com/juanro49/recursos_es-ext/graphs/contributors)

---

# N'Estremeñu

Pendiente de traducir readme al extremeño
