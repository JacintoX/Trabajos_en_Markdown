# Gestores de contenido (CMS)

> **Autor:** Jacinto Rodríguez  
> **Actividad:** CMS, SSG y Markdown

---

## Índice

1. [¿Qué es un CMS?](#qué-es-un-cms)
2. [¿Cómo funciona?](#cómo-funciona)
3. [Ventajas e inconvenientes](#ventajas-e-inconvenientes)
4. [Tipos de CMS y ejemplos](#tipos-de-cms-y-ejemplos)
5. [Los CMS más usados](#los-cms-más-usados)
6. [CMS dinámico frente a SSG](#cms-dinámico-frente-a-ssg)
7. [Vídeo explicativo](#vídeo-explicativo)

---

## ¿Qué es un CMS?

**CMS** significa *Content Management System*, es decir, ***Sistema de Gestión de Contenidos***.

Es un software que permite **crear, modificar, organizar y publicar** contenido en una web mediante una *interfaz de administración*, sin necesidad de escribir el código HTML directamente.

### ¿Para qué sirve?

Sirve para administrar una web y su contenido de una manera más sencilla: el CMS se encarga de gestionar todo ese contenido por nosotros.

## ¿Cómo funciona?

Los contenidos son lo que queremos mostrar a los visitantes. El proceso habitual es:

1. Escribimos el **título** y el **texto**.
2. Añadimos una imagen.
3. Pulsamos el botón `Publicar`.
4. El CMS:
   - guarda la información en una **base de datos**,
   - y la muestra en la web cuando alguien la visita.

Además de crearlos, desde el panel también se pueden:

- Modificar
- Organizar
- Publicar
- Eliminar

![Funcionamiento de un CMS dinámico](img/proceso_cms.png)

De forma muy simplificada, lo que hace un CMS como WordPress cuando llega una visita se parece a esto (pseudocódigo en PHP):

```php
<?php
// El HTML se genera en el momento de la petición
$entrada = $db->query("SELECT titulo, texto FROM entradas WHERE id = 1");
echo "<h1>" . $entrada['titulo'] . "</h1>";
echo "<p>" . $entrada['texto'] . "</p>";
?>
```

## Ventajas e inconvenientes

### Ventajas

- **Velocidad** de desarrollo y mantenimiento.
- Muchos son de ~~pago~~ **código abierto**.
- Funcionalidades avanzadas: formularios, mapas, calendario de eventos, etc.
- Fáciles de usar para personas con poca o ninguna habilidad técnica.
- Reducen costes: cuando los usuarios aprenden a usarlo, se desenvuelven solos y se necesita menos asistencia técnica.
- Disponen de una gran comunidad, que les da *robustez* y *fiabilidad*.

### Inconvenientes

- **Costes de implementación** para adaptarlo a las necesidades del usuario (plugins, temas, etc.).
- Consumo de **recursos del servidor**, que en casos extremos puede provocar su caída.
- Si los usuarios no aprenden los conceptos básicos del CMS, su uso no es eficiente y puede hacer falta contratar ayuda técnica.
- **Mantenimiento:** si no se actualiza periódicamente, pueden aparecer graves vulnerabilidades de seguridad.
- **Soporte técnico:** en plataformas mantenidas por la comunidad hay que confiar en foros y documentación.

> ⚠️ **Importante:** un CMS desactualizado es una de las puertas de entrada más habituales para los ataques.
>
> > Por eso conviene mantener al día el núcleo, los temas y los plugins.

## Tipos de CMS y ejemplos

Los CMS se clasifican según su **propósito**, su **licencia** y su **arquitectura**.

### Según su propósito

| Propósito | Descripción | Ejemplos |
| :-------- | :---------- | :------- |
| General | Priorizan la facilidad para publicar texto, imágenes y vídeo | WordPress, Joomla, Drupal |
| Comercio electrónico | Tiendas online con pasarela de pago, inventario, envíos y carrito | Shopify, PrestaShop, Magento/Adobe Commerce |
| Educación | Cursos online, alumnos, calificaciones y material | Moodle |
| Foros y comunidades | Hilos de discusión, perfiles, reputación y moderación | Discourse, phpBB |

### Según su arquitectura

#### Monolítico (tradicional o acoplado)

Une el *backend* y el *frontend* en un solo sistema. Ejemplos: **WordPress**, **Joomla**, **Drupal**.

#### Desacoplado

Separa el *backend* del *frontend*, pero incluye una capa de presentación predeterminada. Ejemplos: **Magnolia**, **Drupal desacoplado** (por ejemplo, con Acquia).

#### Headless

Elimina por completo la capa visual: solo almacena la información de forma estructurada y la distribuye mediante **APIs** a cualquier dispositivo. Ejemplos: **Strapi**, **Sanity**, **Contentful**.

##### Resumen de arquitecturas

- [x] Monolítico → backend + frontend juntos
- [x] Desacoplado → separados, con frontend incluido
- [x] Headless → solo backend + API
- [ ] Elegir CMS para la práctica final

###### Nota: la clasificación por licencia distingue entre CMS de código abierto y CMS propietarios.

## Los CMS más usados

Según **W3Techs**[^1], consultado el 16 de septiembre de 2026, el top 5 de CMS a nivel mundial es:

| Puesto | CMS | Cuota |
| :----: | :-- | ----: |
| 1 | WordPress | 58,8 % |
| 2 | Shopify | 7,8 % |
| 3 | Wix | 6,2 % |
| 4 | Squarespace | 3,5 % |
| 5 | Joomla | 1,6 % |

![Top 5 CMS más usados](img/cuota_cms.png)

## CMS dinámico frente a SSG

La gran diferencia es **cuándo se genera el HTML**: en un SSG ya está creado antes de recibir las visitas; en un CMS dinámico se genera cuando llega la petición.

| Aspecto | CMS dinámico | Generador de sitios estáticos (SSG) |
| :------ | :----------- | :---------------------------------- |
| Generación del HTML | En cada petición | Antes, durante el *build* |
| Base de datos | Sí | No |
| Edición del contenido | Panel de administración | Archivos (normalmente Markdown) |
| Velocidad | Depende del servidor | Muy rápida |
| Seguridad | Más expuesto (plugins, BD) | Menos superficie de ataque |
| Perfil de usuario | Sin conocimientos técnicos | Conocimientos técnicos básicos |
| Funciones dinámicas | Incluidas | Requieren tecnologías adicionales |
| Ejemplos | WordPress, Joomla, Drupal | Jekyll, Hugo, Astro |

Puedes ver la explicación completa de los generadores de sitios estáticos en el documento [ssg.md](ssg.md).

## Vídeo explicativo

Vídeo de menos de 5 minutos: [Qué es un CMS y para qué sirve (Explicado en 2 minutos)](https://www.youtube.com/watch?v=sSh5AAmItN0)

[![Vídeo: Qué es un CMS](https://img.youtube.com/vi/sSh5AAmItN0/0.jpg)](https://www.youtube.com/watch?v=sSh5AAmItN0)

---

[^1]: W3Techs — Usage statistics of content management systems: <https://w3techs.com/technologies/overview/content_management>
