# Autoencoders


## Entendiendo los Autoencoders - Parte I: Introducción y espacios latentes

El aprendizaje profundo generativo es un campo que ha capturado la atención de muchos investigadores y entusiastas. A medida que se exploran y descubren nuevos diseños de redes neuronales de aprendizaje profundo generativo, se ha identificado la necesidad de compartir estos conocimientos con una audiencia más amplia. Esta sección se sumerge en una arquitectura neural específica: el autoencoder.

### Historia ilustrativa: El estilista y el armario mágico

David Foster, en su [2ª edición de Generative Deep Learning](https://www.oreilly.com/library/view/generative-deep-learning/9781098134174/), presenta una historia que ilustra conceptos complejos del aprendizaje profundo. Imaginemos un escenario en el que alguien trabaja con un estilista llamado Brian. Brian se frustra porque le lleva mucho tiempo encontrar ciertas prendas de ropa debido a que todo está en el suelo en un gran montón. Para solucionar este problema, Brian propone organizar la ropa en un armario mágico que es infinitamente alto y ancho. Una vez organizada la ropa, se puede indicar a Brian la ubicación de una prenda, y él la creará desde cero.

El desafío radica en cómo organizar y describir la ropa en este armario mágico. Es esencial colocar artículos similares cerca uno del otro para que Brian pueda recrearlos con precisión. Con el tiempo, al entender mejor el armario, Brian puede crear prendas que se asemejan a lo que se le ha solicitado. Lo más sorprendente es que Brian puede generar prendas completamente nuevas que nunca han existido antes, simplemente eligiendo un lugar vacío en el armario infinito y dejando que Brian trabaje su magia.

### Espacio latente: Una explicación

El concepto detrás de la historia del estilista es el "espacio latente". Imaginemos un conjunto de alimentos enlatados comunes en supermercados. Estas latas varían en forma y tamaño. Al analizar imágenes de estas latas, la dimensionalidad de todas estas latas se describe por la suma de todos los píxeles. Sin embargo, en lugar de describir la lata usando miles de píxeles, se podría describir la imagen con dimensiones más bajas, como el ancho y el alto. Esta reducción de la dimensionalidad es lo que se conoce como "espacio latente".

![Ejemplo de un espacio latente](https://miro.medium.com/v2/resize:fit:1400/format:webp/0*3BFRAEBNQRHuJfSK.png)


### Aplicación en Autoencoders

En el contexto de los autoencoders, describir la ropa en una dimensionalidad más baja se llama "codificador" y el proceso de tomar esa descripción y recrear el objeto en su dimensionalidad original se llama "decodificador". En futuras secciones, se explorará más a fondo cómo funcionan ambas partes y cómo implementar el autoencoder en PyTorch en Python.

Fuente: https://blog.gopenai.com/understanding-autoencoders-part-i-introduction-and-latent-spaces-69cbe68b6fda