# Curso básico de Git y Github

## ¿Qué es Git?

Es un software de control de versiones diseñado por Linus Torvalds, pensando en
la eficiencia y la confiabilidad del mantenimiento de versiones de aplicaciones
cuando éstas tienen un gran número de archivos de código fuente. Su propósito es
llevar registro de los cambios en archivos de computadora y coordinar el trabajo
que varias personas realizan sobre archivos compartidos.

## ¿Por qué Git?

-   Desarrollo no lineal
-   Gestión distribuida
-   Gestión eficiente para proyectos
-   Menos almacenamiento necesario

## ¿Qué es Github?

GitHub es una plataforma de desarrollo colaborativo, para alojar proyectos
utilizando el sistema de control de versiones Git. Se utiliza principalmente
para la creación de código fuente de programas de ordenador.

## Primeros comandos de Git

### Configurando Git

| Comando                                    | Para qué sirve                                      |
| ------------------------------------------ | --------------------------------------------------- |
| git --version                              | Revisamos la versión actual de Git                  |
| git config --global user.email “Tu correo” | Configuramos el correo del usuario                  |
| git config --global user.name “Tu nombre”  | Configuramos el nombre del usuario                  |
| git config --list                          | Revisamos que nuestras configuraciones se guardaron |

### Nuestro primer repositorio

| Comando                            | Para qué sirve                                       |
| ---------------------------------- | ---------------------------------------------------- |
| git init                           | Inicializamos el repositorio                         |
| git status                         | Observamos el status de nuestro repositorio          |
| git add historia.txt               | Añadimos un nuevo archivo al staging del repositorio |
| git commit -m “Mensaje del commit” | Realizamos el commit al repositorio                  |

### Revisando los cambios en el repositorio

| Comando               | Para qué sirve                                              |
| --------------------- | ----------------------------------------------------------- |
| git log historia.txt  | Revisamos los commits hechos en un archivo                  |
| git show historia.txt | Revisamos los últimos cambios hechos a un archivo           |
| git diff a b          | Revisamos los cambios hechos de la versión a a la versión b |

### Viajando en el tiempo

| Comando                      | Para qué sirve                              |
| ---------------------------- | ------------------------------------------- |
| git checkout “ID del commit” | Viajamos al estado del commit que indicamos |

**Advertencia:** Hacer un commit en un punto que no sea el head del master,
puede causar pérdida de los archivos. Hazlo solo si deseas continuar desde ese
punto y olvidar todos los cambios anteriores.
