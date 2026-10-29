# Reto 1: Solucion Iterativa de Jacobi para la Ecuacion de Poisson

Este proyecto implementa la solucion numerica de la Ecuacion de Poisson en 2D utilizando el metodo iterativo de Jacobi. El objetivo principal es analizar y comparar el rendimiento de diferentes estrategias de optimizacion a nivel de memoria y modelos de ejecucion paralela en sistemas de Computacion de Alto Rendimiento (HPC).

---

## Estructura del Proyecto

```text
.
├── HPC-Jacobi-reto1/
│   ├── Makefile                # Script para la compilacion automatizada
│   ├── benchmark.sh            # Script de ejecucion y medicion de tiempos
│   └── src/
│       ├── poisson.h           # Archivo de cabecera con constantes y prototipos
│       ├── poisson.c           # Logica basica del algoritmo de Poisson
│       ├── serial_std.c        # Implementacion secuencial estandar
│       ├── serial_cache.c      # Implementacion secuencial optimizada para memoria cache
│       ├── threads.c           # Implementacion paralela basada en hilos
│       └── processes.c         # Implementacion paralela basada en procesos
├── summary_serial.txt          # Resumen de metricas de la ejecucion secuencial
├── summary_threads.txt         # Resumen de metricas de la ejecucion con hilos
└── summary_processes.txt       # Resumen de metricas de la ejecucion con procesos
