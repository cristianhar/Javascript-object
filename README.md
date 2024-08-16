## Herencia en Clases, Polimorfismo y Encapsulamiento

En esta sección del proyecto, se exploran conceptos fundamentales de la programación orientada a objetos en JavaScript, incluyendo **herencia en clases**, **polimorfismo** y **encapsulamiento**. A continuación, se detallan los archivos y ejemplos que ilustran estos conceptos.

### 1. Herencia en Clases

**Descripción**: La herencia en clases permite que una clase derive de otra, reutilizando y extendiendo su funcionalidad. En JavaScript, esto se logra mediante la palabra clave `extends`. La clase hija hereda propiedades y métodos de la clase padre y puede sobrescribir o añadir nuevas funcionalidades.

**Archivos**:
- `Persona.js`
- `Estudiante.js`
- `FiguraGeometrica.js`

**Ejemplos**:

- **Clase `Persona`**: Clase base que incluye propiedades y métodos básicos como `nombre`, `edad` y `fechaNacimiento`.
- **Clase `Estudiante`**: Hereda de `Persona` y añade una propiedad `grado`. También sobrescribe el método `toString` para incluir información adicional.
- **Clase `FiguraGeometrica`**: Clase base para diferentes figuras geométricas, con propiedades `nombre` y `color`.
- **Clases `Rectangulo` y `Circulo`**: Heredan de `FiguraGeometrica` y añaden propiedades específicas y métodos para calcular área y perímetro.

### 2. Polimorfismo

**Descripción**: El polimorfismo permite que una misma interfaz o método se comporte de manera diferente en diferentes contextos. En JavaScript, el polimorfismo se manifiesta cuando una clase hija sobrescribe un método de la clase base. Esto permite que el mismo método tenga diferentes implementaciones dependiendo de la clase que lo utilice.

**Archivos**:
- `Estudiante.js`
- `Empleado.js`

**Ejemplos**:

- **Método `realizarTarea` en `Estudiante` y `EstudianteTrabajador`**: La clase `Estudiante` tiene un método `realizarTarea` que es sobrescrito en la clase `EstudianteTrabajador`, demostrando cómo el mismo método puede comportarse de manera diferente en función de la clase.
- **Método `realizarTarea` en `Empleado`, `Gerente` y `Vendedor`**: Las clases `Gerente` y `Vendedor`, que heredan de `Empleado`, sobrescriben el método `realizarTarea` para proporcionar comportamientos específicos para cada tipo de empleado.

### 3. Encapsulamiento

**Descripción**: El encapsulamiento es una técnica que oculta los detalles internos de una clase y expone solo lo necesario a través de métodos públicos. En JavaScript, se puede lograr encapsulamiento usando propiedades privadas (con el prefijo `#`) y métodos públicos para acceder o modificar estas propiedades.

**Archivos**:
- `Persona.js`
- `Estudiante.js`
- `FiguraGeometrica.js`

**Ejemplos**:

- **Propiedades Privadas en `Persona`**: Las propiedades `#nombre`, `#edad`, y `#fechaNacimiento` están encapsuladas y sólo accesibles a través de métodos públicos como `obtenerNombre`, `obtenerEdad`, y `obtenerFechaNacimiento`.
- **Métodos Privados en `FiguraGeometrica`**: Las propiedades `#nombre` y `#color` están encapsuladas y solo se accede a ellas mediante métodos públicos como `establecerNombre` y `obtenerNombre`.
