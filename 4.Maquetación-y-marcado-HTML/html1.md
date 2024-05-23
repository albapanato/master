## UNIDAD 4 - Maquetación y marcado HTML

1. [Conceptos básicos I](#1-conceptos-básicos-i)

2. [Conceptos básicos II](#2-)

3. [Elementos: Listados en HTML5]

4. [Elementos: Tablas en HTML5]

5. [Elementos: Enlaces en HTML5]

6. [Elementos: Imágenes]

7. [Creación y gestión de formularios]

---

## 1. Conceptos básicos I:

### 1.1 ¿Qué es y cómo funciona HTML?

No es un lenuaje de programacion, sino un lenguaje de marcado.

HTML son las siglas de Hyper Text Markup Language

### Etiqueta `<!DOCTYPE html>`

Para abrir la etiqueta para crear una pagina con html

### Etiqueta `<html lang="en">`

Para que salga la opcion de cambiar el idioma en las paginas

### Etiquetas `<head>`

<meta charset="UTF-8"> -----> configura los caracteres de una pagina, como por ejemplo las ñ o acentos.

<meta name="author" content=" Alba"></meta> ---> Va el autor de la pagina.

### Etiquetas `<body>`

<form> ---> GET lleva los datos de forma "visible" al cliente (navegador web). El medio de envío es la URL. Los datos los puede ver cualquiera. POST consiste en datos "ocultos" (porque el cliente no los ve) enviados por un formulario cuyo método de envío es post.

<form action="back/usuario/nuevoUsuario.php" method="get/post">

<h2>Mi formulario</h2>
  <div>
      <label for="IDNombre">Dime tu nombre:</label>
      <input
        name="nombre"
        type="text"
        id="IDNombre"
        placeholder="Pon tu nombre"----> para que aparezca el texto en color clarito y que cuando pinchas en el input se elimina
      />
    </div>
<div>
    Contraseña:
    <input name="pwd" type="password" /> ---> se puede añadir disabled o required
        <input name="pwd" type="password" required />
        <input name="pwd" type="password" disabled />

</div>
<div>
    Icono de empresa:
    <input
    type="file"
    name="input type file para buscar accept"
    id=""
    accept="image/png,image/jpeg"
    multiple
    />
</div>
    <div>
    Tu color favorito:
    <select name="color" id="">
    <option value="verde">Verde</option>
    <option value="azul">Azul</option>
    <option value="amarillo">Amarillo</option>
    </select>
</div>

Como nos has conocido?

<div>
    <input type="radio" name="gente" id="radio1" /> ----> con input type="radio" sale un punto para seleccionar.
    <label for="radio1"> gente</label>
</div>
<div>
    <input type="radio" name="television" id="radio2" />
    <label for="radio2"> television</label>
</div>
<div>
    <input type="radio" name="univerdidad" id="radio3" />
    <label for="radio3"> universidad </label>

</div>

<div>
      <label for="textarea">Danos tu opinion:</label><br>
      <textarea name="" id="textarea" cols="30" rows="10"></textarea> ----> se puede editar el numero de cols y de rows
    </div>

<button type="submit">Enviar</button>

</form>

SEO valora:

<img>----> alt= "Rellenar con una frase" y agregar title=" lo que aparecera cuando pasamos con el raton encima de a imagen"

        <img src="" alt="" title="">

<a>-----> lo mismo que con img. Preferible rellenar o añadir siempre un title.
<a title="" href=""></a>
