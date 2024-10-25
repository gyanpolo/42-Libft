# Libft

**Libft** es uno de los proyectos básicos del currículo de la Escuela 42, cuyo objetivo es crear una librería en C desde cero. Esta librería contiene una serie de funciones estándar que replican y amplían funcionalidades de la biblioteca estándar de C (`<string.h>`, `<stdlib.h>`, `<ctype.h>`, entre otras). Libft es la primera piedra en la construcción de habilidades sólidas en C, ya que los proyectos futuros pueden requerir el uso de esta librería personalizada.

## Objetivos

- **Implementar funciones estándar en C**: Replicar el comportamiento de funciones comunes de la biblioteca estándar para comprender su funcionamiento a fondo.
- **Construir una librería reutilizable**: Crear una colección de funciones que pueden usarse en proyectos futuros.
- **Fortalecer fundamentos en C**: Practicar el manejo de memoria, punteros, estructuras y control de flujo en C.

## Contenidos del Proyecto

El proyecto Libft se divide en tres secciones principales:

### 1. **Funciones de la Biblioteca Estándar**

Estas funciones replican funcionalidades básicas de `<string.h>`, `<ctype.h>`, entre otras:

- `ft_memset`, `ft_bzero`, `ft_memcpy`, `ft_memmove`: Manipulación de bloques de memoria.
- `ft_strlen`, `ft_strdup`, `ft_strcpy`, `ft_strncpy`: Funciones de manejo de cadenas.
- `ft_atoi`, `ft_isalpha`, `ft_isdigit`, `ft_isalnum`: Funciones de conversión y comprobación de caracteres.

### 2. **Funciones Adicionales**

Funciones que no forman parte de la biblioteca estándar, pero que pueden ser útiles en una amplia variedad de proyectos, como:

- `ft_substr`, `ft_strjoin`, `ft_strtrim`: Funciones para manipular y combinar cadenas.
- `ft_split`: Divide una cadena en palabras en función de un delimitador.
- `ft_itoa`: Convierte un entero en una cadena.

### 3. **Funciones de Lista Enlazada (Opcional)**

Funciones para trabajar con listas enlazadas simples, como:

- `ft_lstnew`: Crea un nuevo nodo.
- `ft_lstadd_front`, `ft_lstadd_back`: Añade un nodo al principio o al final de la lista.
- `ft_lstsize`: Calcula el tamaño de la lista.
- `ft_lstdelone`, `ft_lstclear`: Elimina nodos de la lista.

## Instalación y Uso

1. Clona el repositorio de Libft en tu máquina local:

    ```bash
    git clone https://github.com/gyanpolo/42-Libft.git
    cd 42-Libft
    ```

2. Compila la librería:

    ```bash
    make
    ```

3. Se generará un archivo `libft.a` que podrás incluir en tus proyectos. Compila tu código enlazando `libft.a` para usar las funciones de Libft.

## Ejemplo de Uso

```c
#include "libft.h"

int main() {
    char *str = "42 Barcelona";
    int len = ft_strlen(str);

    ft_putstr("La longitud de la cadena es: ");
    ft_putnbr(len);
    ft_putchar('\n');

    return 0;
}
