# Sección 01: Ejemplo 01.Modelo de caja
## BOX-SIZING

Ejemplos en el que vemos los tres casos de ´*BOX-SIZING*.
En 1 lugar tenemos una caja donde le ponemos un padding y un border sin establecer las propiedades de ´*BOX-SIZING*´.
```
div{
 
    width: 20rem;
    height: 20rem;
    background-color: salmon;
    padding: 5rem;
    border: 20px solid blue;
}
```

En 2 lugar tenemos una caja donde le ponemos un padding y un border estableciendo el  '*box-sizing: content-box*´.Donde se ven los primeros cambios al usar este modelo.

```
div{
    box-sizing: content-box;
    width: 20rem;
    height: 20rem;
    background-color: salmon;
    padding: 5rem;
    border: 20px solid blue;
}
````

En 3 lugar tenemos una caja donde le ponemos un padding y un border estableciendo el  '*box-sizing: padding-box*´.Donde se ven que el padding hace que el tamñano de la caja aumente.

````
div{
    box-sizing: content-box;
    width: 20rem;
    height: 20rem;
    background-color: salmon;
    padding: 5rem;
    border: 20px solid blue;
}
````

En 4 lugar tenemos una caja donde le ponemos un padding y un border estableciendo el  '*box-sizing: ´border-box*´.Donde se que este modelo hace qu se mantenga su tamaño original y lo q no entre en la caja sobresalga.Una solución para este problema es utilizar el overflow.

````
div{
    box-sizing: border-box;
    width: 20rem;
    height: 20rem;
    background-color: salmon;
    padding: 5rem;
    border: 20px solid blue;
    overflow: auto;
}
````