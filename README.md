# Prácticas de Laboratorio de Sistemas Informáticos Industriales (SII)

**Autor:** Andrés Galindo Gordón  
**Matrícula:** 56939

Este es un repositorio que contiene el código C++ de las prácticas de laboratorio para el desarrollo del juego de tenis mediante OpenGL y GLUT.

## Implementaciones

* **Práctica 1 - Entorno Linux:** Configuración del entorno en Linux utilizando Git y CMake. El código inicial requería incluir el código relativo al movimiento de las raquetas mediante el teclado (tanto para el jugador 1 como para el jugador 2), además del movimiento de la esfera.

* **Práctica 2 - Tuberías FIFO:** Se creó un proceso independiente llamado `logger.cpp` trabajando con la creación de tuberías para comunicar procesos independientes. El *logger* se encarga de mostrar por pantalla el recuento de puntos de cada jugador en tiempo real. Además, la partida llega a su fin y se cierran los procesos cuando uno de los jugadores alcanza los 3 puntos.

* **Práctica 3 - Memoria Compartida (`mmap`):** Se ha implementado un proceso que permite que la raqueta izquierda juegue de manera autónoma (`bot.cpp`). Esta IA modificará su movimiento vertical dependiendo de la posición de la pelota relativa al centro de su raqueta, subiendo o bajando en cada caso. Se crea un fichero proyectado en memoria para que tanto el bot como el motor del juego puedan acceder a este, consultar la posición de la pelota y tomar las decisiones correspondientes en cada momento.
