# Integración de Inteligencia Artificial

## Descripción General

Uno de los componentes principales de MAMBAQ Interactivo es la integración de un modelo de Inteligencia Artificial capaz de clasificar imágenes cargadas por los usuarios.

Esta funcionalidad fue desarrollada utilizando Teachable Machine, una plataforma creada por Google que permite entrenar modelos de aprendizaje automático sin necesidad de programar redes neuronales desde cero.

El objetivo de esta herramienta es ofrecer una experiencia educativa e interactiva para niños y jóvenes, permitiéndoles subir imágenes de sus obras y obtener una clasificación automática.

---

## Entrenamiento del Modelo

Para el entrenamiento del modelo se utilizó la modalidad de clasificación de imágenes de Teachable Machine.

Se definieron cinco categorías principales:

- Personas
- Animales
- Paisajes
- Vehículos
- Construcciones

Cada categoría fue alimentada con 50 imágenes de entrenamiento para mejorar la precisión de las predicciones realizadas por el modelo.

---

## Proceso de Entrenamiento

El proceso de creación del modelo siguió las siguientes etapas:

1. Creación de las clases de clasificación.
2. Recolección de imágenes para cada categoría.
3. Entrenamiento del modelo mediante Teachable Machine.
4. Evaluación de resultados.
5. Exportación del modelo en formato TensorFlow.js.
6. Integración dentro de la aplicación web.

![Modelo Entrenado](/img/script_IA.png)

---

## Integración con la Página Web

Una vez exportado el modelo, se generaron los siguientes archivos:

- model.json
- metadata.json
- Archivos binarios de pesos del modelo

Estos archivos fueron almacenados dentro de la carpeta:

```text
ModeloIA/
```

La aplicación utiliza TensorFlow.js y la librería de Teachable Machine para cargar el modelo directamente desde el navegador.

---

## Funcionamiento

Cuando el usuario selecciona una imagen y presiona el botón "Analizar con IA", el sistema realiza las siguientes acciones:

1. Carga la imagen seleccionada.
2. Ejecuta el modelo de clasificación.
3. Obtiene las probabilidades de cada categoría.
4. Selecciona la categoría con mayor nivel de confianza.
5. Muestra el resultado al usuario.

Posteriormente, la obra puede almacenarse dentro de la galería de visitantes junto con la categoría detectada.

![IA Funcionando](/img/prueba.png)

---

## Beneficios de la Implementación

La integración de Inteligencia Artificial permitió:

- Incorporar aprendizaje automático dentro del proyecto.
- Crear una experiencia interactiva para los usuarios.
- Clasificar automáticamente las obras cargadas.
- Combinar arte, educación y tecnología dentro de una misma plataforma.

---

## Tecnologías Utilizadas

- Teachable Machine
- TensorFlow.js
- JavaScript
- HTML5
- CSS3