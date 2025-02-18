# Philosophers

![C Language](https://img.shields.io/badge/C-Programming-blue.svg) ![Makefile](https://img.shields.io/badge/Makefile-Build-orange.svg) ![Git](https://img.shields.io/badge/Git-Version%20Control-red.svg) ![Norminette](https://img.shields.io/badge/Norminette-Code%20Style-brightgreen.svg) ![POSIX Threads](https://img.shields.io/badge/POSIX-Pthreads-yellow.svg) ![OS: Linux](https://img.shields.io/badge/OS-Linux-lightgrey.svg)

## 📌 Descripción

El proyecto **Philosophers** es una implementación del problema de los filósofos comensales, diseñado para comprender y aplicar conceptos de programación concurrente. Su objetivo es evitar bloqueos y condiciones de carrera en aplicaciones multihilo mediante el uso de **mutexes** y **semáforos**.

En este desafío, múltiples filósofos comparten un número limitado de recursos (**tenedores**) y deben coordinarse para evitar **deadlocks** e **inanición**.

## 🛠 Lenguajes y Tecnologías

- **Lenguaje:** C
- **Librerías:** POSIX Threads (**pthreads**)
- **Mecanismos de sincronización:** Mutex y Semáforos
- **Herramienta de compilación:** Makefile

## 💡 Conceptos de Programación Aplicados

- **Programación Concurrente**
- **Sincronización de Hilos**
- **Evitando Deadlocks**
- **Optimización de Recursos Compartidos**

## 📂 Estructura del Proyecto

```
Philosophers
├── README.md
└── philo
    ├── Makefile
    ├── inc
    │   └── philo.h
    └── src
        ├── check_args.c
        ├── ft_atoi.c
        ├── ft_isdigit.c
        ├── ft_putnbr_fd.c
        ├── ft_putstr_fd.c
        ├── init.c
        ├── main.c
        ├── monitor.c
        ├── philo_routine.c
        ├── threads.c
        └── utils.c
```

## 🚀 Instalación y Uso

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/RikiGuerrero/Philosophers.git
   cd Philosophers
   cd philo
2. Compilar el proyecto:
   ```bash
   make
   ```
3. Ejecutar:
   Para ejecutar el programa usa:
   ```bash
   ./philo <número_de_filósofos> <tiempo_para_morir> <tiempo_para_comer> <tiempo_para_dormir> [número_de_comidas]
   ```
   Ejemplo:
   ```bash
   ./philo 5 800 200 200
   ```
   Donde:
   - ``número_de_filósofos``: Cantidad de filósofos en la mesa.
   - ``tiempo_para_morir``: Tiempo en milisegundos antes de que un filósofo muera si no come.
   - ``tiempo_para_comer``: Tiempo en milisegundos que un filósofo tarda en comer.
   - ``tiempo_para_dormir``: Tiempo en milisegundos que un filósofo pasa durmiendo.
   - ``[número_de_comidas]`` *(opcional)*: Número de comidas que cada filósofo debe completar antes de que el programa finalice.

## ✅ Normas y Estilo de Código

El código sigue las reglas de la **Norminette**, la herramienta de estilo de 42. Para verificar:
```bash
norminette
```

## 📜 Licencia

Este proyecto es parte del currículo de 42 y sigue las reglas de la escuela.
