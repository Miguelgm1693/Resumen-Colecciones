# Resumen-Colecciones
## ¿Qué es una colección en Java? ##

Una colección es un contenedor de elementos de un solo tipo, recoge en una sola unidad.

Su uso puede ser para almacenamieto, recuperación y manipulación de datos. Instancias de otro objeto de una manera conjunta.
Son elementos que forman grupos naturales. _Ejemplo: Un buzón de correo (colección de mensajes)._

Las colecciones ofrecen los siguientes elementos:
- Interfaces.
- Implementaciones.
- Algoritmos.

Las **ventajas** de usar frameworks de colecciones pueden ser:
- Reduce el esfuerzo de programación
- Aumenta la calidad y velocidad de programar
- Interoperabilidad con librerías de terceros
- Reduce el esfuerzo para aprender y usar otras librerías
- Reduce el esfuerzo para diseñar nuevas librerías
- Fomenta la reutilización de software

## Tipos de colecciones ##

### Iterable <E> ###
  
  Concepto de Iterador.
  
  - Patrón de diseño que nos permite recorrer y eliminar elementos.
  - Nos permite usar forEach y el bucle tipo for-each.
  
### Collection <E> ###
  
  - Extiende a _Iterable <E>_ (hereda su funcionalidad)
  - Representa un grupo de elementos
  - Todas las interfaces heredan de él menos Map y derivados
  - Sirve para manipular colecciones de manera general
  
### Set <E> ###
  
  - Trata de un _Collection<E>_ no permite duplicados
  - No hay acceso posicional
  - Mejora implementación de los métodos _equals_ y _hashCode_
  
  **Implementaciones de Set<E>**
  - LinkedHashSet<E> --> Orden de inserción. Almacena valores en una tabla hash con una lista doblemente enlazada
  - HashSet<E> --> Más rápido. Almacena valores en una tabla hash
  - TreeSet<E> --> Orden según valor. Almacena sus valores en un árbol _red-black_. Peor rendimiento que resto de opciones
  
### List <E> ###
  
  - Trata de un _Collection<E>_ permite duplicados.
  - Añade funcionalidades de _Collection<E>_:
  
    · Acceso posicional
    
    · Búsqueda
    
    · Iteración extendida
    
    · Operaciones sobre un rango de elementos de la lista
    
   **Implementaciones de List<E>**
  - ArrayList<E> --> Más adecuada en la mayoría de situaciones
  - Vector<E> --> Sincroniza, pero con métodos _legacy_. Menos recomendable
  - LinkedList<E> --> Eficiente en algunas situaciones
  
   **Otras interfaces relacionadas con List<E>**
  - Queue<E>
  - Deque<E>
  
### Map <K,V> ###

  - No hereda de _Collection<E>
  - Maneja pares clave, valor
  - Para cada clave hay un solo valor
  - Cada clave puede existir una sola vez en map
  - Se le conoce en otros lenguajes como diccionario
  - No almacena tipos primitivos
  
  **Map.Entry<K,V>**
  - Permite consultar un par clave, valor de un Map
  - No se puede utilizar para insertar valores
  
  **Implementaciones Map<K,V>**
  
  - LinkedHashMap<K,V> --> Orden de inserción. Rendimiento un poco peor que HashMap. Ordena los pares clave, valor segun su inserción
  - HashMap<K,V> --> La más utilizada, más rápido. Ejecución constante.
  - TreeMap<K,V> --> Orden según las claves. Peor rendimiento de las 3. Mantiene las claves en orden (natural)
  
## Colecciones no modificables ##

- Colecciones que, una vez creada, no se pueden modificar
- Si se trata de modificar, se lanza UnsupportedOperationException

## Colecciones sincronizadas ##

- Aptas para el uso de diferentes hilos de ejecución.
- Varios procesos / hilos que compiten por el uso de la colección

## Implementaciones menos usadas ##
- Set: 

     · EnumSet
      
     · CopyOnWriteArraySet
      
 
  
    
  





