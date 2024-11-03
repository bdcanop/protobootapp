# Taller de CI/CD

Este repositorio contiene la evidencia del taller de CI/CD, donde se implementaron dos pipelines: uno con **GitHub Actions** y otro con **Jenkins**. Ambos están configurados para ejecutar pruebas cada vez que se hace un push en el repositorio, permitiendo una integración continua de los cambios.

---

## 1. Pipeline de GitHub Actions

### Descripción
El pipeline de GitHub Actions está configurado para ejecutarse automáticamente en cada push, asegurando que las pruebas se ejecuten sin intervención manual.

### Evidencia

#### Se genera un bug en la función cuadrado al modificar el comportamiento de esta multiplicando el resultado por 3, se hace push

<img width="1268" alt="Pasted Graphic 2" src="https://github.com/user-attachments/assets/681cbbe4-d847-4a62-bade-774589122d8f">


#### Falla el build por bug 

![Pasted Graphic](https://github.com/user-attachments/assets/9a8bdd5c-95ba-471c-a851-2f8ae3a4c545)

#### Falla la build debido a error en la función cuadrado de calculadora

![Pasted Graphic 1](https://github.com/user-attachments/assets/a45735e2-949c-4898-8d2e-419e0cfd8ce6)

#### Arreglo el bug y subo los cambios

<img width="1268" alt="Pasted Graphic 5" src="https://github.com/user-attachments/assets/5201d602-8509-43f0-a92b-b48e7c404a8b">

#### Se carga la build

![Pasted Graphic 3](https://github.com/user-attachments/assets/fe116b68-5a15-4d36-a40d-c1783db1fcb8)

#### La build pasa

![Pasted Graphic 4](https://github.com/user-attachments/assets/c516d41f-6f9e-4e1d-aa76-f85380cbcb20)


---

## 2. Pipeline de Jenkins

### Descripción
El pipeline de Jenkins también se ejecuta automáticamente cada que detecte cambios y estos cambios son buscados cada 5 minutos para proporcionar un entorno de integración continua independiente.

### Evidencia

#### El work en Jenkins falla debito al bug de la calculadora

![Pasted Graphic 6](https://github.com/user-attachments/assets/5f34dedb-d0fa-4115-8fb0-d30be5076424)


#### Tras arreglar el bug, el work en Jenkins corre y se pueden ver los detalles

![Jenkins](https://github.com/user-attachments/assets/1e17b83e-f097-4d8e-948f-be0d0e08a9b7)


---

## Conclusión

Ambos pipelines permiten realizar una integración continua mediante la ejecución automática de pruebas con cada push al repositorio. Esto contribuye a una mayor confianza en los cambios realizados y facilita la detección temprana de errores.
