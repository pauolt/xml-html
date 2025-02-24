# HE TENIDO QUE MODIFICAR EL XML Y DTD PORQUE SINO ERA COMPLETAMENTE INFUMABLE. DEMASIADO EXTENSO.
# Grieta del Invocador - Campeones

Este archivo XML describe varios campeones del juego **League of Legends** y sus habilidades. A continuación se explica cada sección y sus componentes.

## Estructura General

El archivo está compuesto por un solo elemento raíz llamado `<grieta_del_invocador>`. Dentro de este elemento, se encuentran los detalles de varios campeones.

### `campeones`

Es un contenedor que agrupa todos los campeones de la Grieta del Invocador. Cada campeón está representado por el elemento `<campeon>`, el cual contiene diversos atributos y elementos hijos.

### Atributos de `<campeon>`

- **recurso**: Este atributo indica el tipo de recurso que utiliza el campeón, como **mana** o **energía**.
- **clase**: Define el rol o clase del campeón, como **tirador**, **luchador**, **tanque**, **soporte**, entre otros.

### Elementos dentro de `<campeon>`

- **nombre**: El nombre del campeón.
- **imagen**: Un elemento con un atributo `url` que contiene el enlace a una imagen del campeón en un sitio web externo.
- **descripcion**: Breve descripción del campeón.
- **habilidades**: Un contenedor que incluye las habilidades del campeón.

## Habilidades

Cada campeón tiene una lista de habilidades representada por el elemento `<habilidad>`. Las habilidades pueden tener los siguientes subelementos:

- **tipo** (opcional): Especifica si la habilidad es de tipo **Pasiva** o **Ultimate**.
- **coste** (opcional): Define el costo de la habilidad en recursos (por ejemplo, **mana**).
- **descripcion**: Descripción detallada de lo que hace la habilidad.

