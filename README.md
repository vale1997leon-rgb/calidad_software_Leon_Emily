# Calidad del Software 
# Autor: Emily Leon 

# Precurso de Calidad de Software

Este repositorio contiene los conceptos básicos de Calidad de Software y las pruebas utilizadas para verificar que una aplicación cumple sus requisitos y funciona correctamente.

## Objetivos

Al finalizar este precurso podrás aprender a:

- Identificar los principales conceptos de calidad de software.
- Diferenciar entre pruebas unitarias, pruebas de integración y pruebas E2E.
- Diseñar casos de prueba efectivos.
- Detectar defectos durante el desarrollo.
- Aplicar buenas prácticas para mantener una aplicación segura, confiable y mantenible.

## Conceptos básicos

### Calidad de Software

La calidad de software es la capacidad de un sistema para satisfacer necesidades funcionales, no funcionales y de mantenimiento. Un software de calidad debe ser:

- **Funcional:** cumple los requisitos definidos.
- **Confiable:** funciona de forma consistente y con pocas fallas.
- **Seguro:** protege los datos y evita riesgos.
- **Mantenerable:** puede ser modificado con facilidad.
- **Eficiente:** utiliza recursos de forma adecuada.
- **Accesible:** puede ser utilizado por personas con distintas necesidades.

### Defecto

Un defecto es un error que impide que el software cumpla un requisito o produce un resultado incorrecto. Cuando un defecto se detecta antes de la entrega se conoce como **defecto**; si se detecta después de la entrega, se considera un **fallo**.

### Requisito

Un requisito describe lo que el sistema debe hacer. Puede ser:

- **Funcional:** qué debe hacer el sistema.
- **No funcional:** cómo debe comportarse el sistema, por ejemplo, su velocidad, seguridad o usabilidad.
- **De restricción:** las limitaciones que debe respetar.

### Ciclo de vida del software

El ciclo de vida suele incluir:

1. Análisis de requisitos.
2. Diseño.
3. Implementación.
4. Pruebas.
5. Instalación y despliegue.
6. Mantenimiento.

### Pruebas de calidad

Una prueba debe comprobar un comportamiento esperado y proporcionar evidencia de que el sistema funciona correctamente. Las pruebas deben ser:

- **Claramente definidas:** describen qué se espera.
- **Repetibles:** producen resultados similares en diferentes ejecuciones.
- **Automatizables:** pueden ejecutarse sin intervención manual.
- **Escalables:** pueden adaptarse a nuevos requisitos.

## Tipos de pruebas

### Pruebas unitarias

Las pruebas unitarias verifican una unidad pequeña de código, normalmente una función, método o clase. Se ejecutan de forma aislada y ayudan a detectar errores antes de que se propaguen a otros componentes.

Entre sus principales ventajas se encuentran:

- Ejecución rápida.
- Detección temprana de errores.
- Mayor cobertura del código.
- Fácil mantenimiento.

Una prueba unitaria debe cubrir:

- El caso feliz.
- Casos de error o excepción.
- Entradas inválidas.
- Limites de los datos.

### Pruebas de integración

Las pruebas de integración verifican la interacción entre componentes. Por ejemplo, se puede comprobar que la base de datos, la API y la interfaz se comunican correctamente.

### Pruebas E2E

Las pruebas E2E, o pruebas de extremo a extremo, verifican el flujo completo de una aplicación como lo utiliza un usuario. Simulan la interacción con la interfaz y con los servicios externos necesarios para completar una tarea.

Por ejemplo, una prueba E2E podría:

1. Abrir la aplicación.
2. Iniciar sesión.
3. Crear un pedido.
4. Confirmar el pedido.
5. Verificar que el pedido aparece en la lista.

Las pruebas E2E son útiles para validar el comportamiento real, pero suelen ser más lentas y depender de un entorno de pruebas adecuado.

## Diferencia entre pruebas unitarias y pruebas E2E

| Característica | Pruebas unitarias | Pruebas E2E |
|---|---|---|
| Alcance | Una unidad pequeña | Flujo completo de la aplicación |
| Ejecución | Rápida y aislada | Más lenta y dependiente de otros servicios |
| Objetivo | Verificar una función | Verificar el comportamiento del usuario |
| Ejemplo | Calcular un descuento | Completar una compra en la aplicación |
| Frecuencia | Alta | Menor frecuencia |

## Buenas prácticas

- Definir casos de prueba antes de implementar.
- Usar datos de prueba claros y pequeños.
- Evitar pruebas que dependan de detalles internos.
- Mantener las pruebas fáciles de entender.
- Ejecutar las pruebas en un entorno limpio.
- Revisar los resultados y corregir los defectos.
- Mantener una documentación actualizada de los requisitos.

## Comandos sugeridos

En este repositorio se pueden añadir scripts para ejecutar las pruebas cuando se implemente el proyecto:

```bash
npm test
npm test:unit
npm test:e2e
```

## Conclusión

La calidad de software no consiste solamente en encontrar errores, sino en prevenirlos, detectarlos temprano y validar el comportamiento correcto del sistema. Las pruebas unitarias y E2E complementan el proceso de desarrollo y ayudan a ofrecer software confiable, seguro y satisfactorio para sus usuarios.
