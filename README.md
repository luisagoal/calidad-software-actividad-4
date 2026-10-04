# Calidad de Software - Actividad 4

Comparación de herramientas de calidad de software (Selenium, Postman, JMeter,
Cypress, Allure y SonarQube) y aplicación práctica de Postman a una simulación
del caso Boeing Starliner (2019).

## Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `Calidad de software Act 4.pdf` | Documento con el análisis completo de la actividad |
| `Starliner - Control de Misión.postman_collection.json` | Colección de Postman con 4 peticiones y 9 pruebas automatizadas |
| `Escenario 2019 (con error).postman_environment.json` | Entorno con los datos que reproducen las fallas del vuelo de 2019 |
| `Escenario corregido.postman_environment.json` | Entorno con los datos correctos |

## Cómo ejecutar las pruebas

1. Descarga los tres archivos `.json` de este repositorio.
2. En Postman, haz clic en **Import** y carga la colección y los dos entornos.
3. Selecciona el entorno **Escenario 2019 (con error)** y ejecuta la colección con el **Collection Runner**.
   - Resultado esperado: **6 pruebas aprobadas y 3 fallidas** (sincronización del reloj, combustible y riesgo de colisión).
4. Cambia al entorno **Escenario corregido** y ejecuta de nuevo.
   - Resultado esperado: **9 de 9 pruebas aprobadas**.

Las peticiones se envían a [Postman Echo](https://postman-echo.com), un servicio de pruebas
oficial de Postman, por lo que no se requiere configuración adicional.

## Autora

Luisa María González Álvarez
Ingeniería de Software, Séptimo Semestre
Corporación Universitaria Iberoamericana
