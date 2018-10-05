# PSP

## Clase
Una clase es como la plantilla base en la cual se utiliza para escribir casi todo el código de java.

Cuando creemos una clase le pondremos un nombre, en este caso le he puesto nombre.

##### Ejemplo
```java
public class nombre {

}
```

## Objeto
En la programación se utiliza mucho la Programación Orientada a Objetos. Como podemos ver en estas tres palabras se orienta mucho con los objetos de la vida cotidiana(pelota, coche, movil, persona). En la vida real tienen características que a estos objetos los hace únicos:  
Pelota  -> Diametro, color, presión, marca.  
Coche   -> Puertas, motor, ruedas, color.  
Movil   -> Marca, modelo, pantalla, camara.  
Persona -> Nombre, apellidos, dni, numeroTelefono.  

Como podemos ver que cada objeto tiene unas característica y esas características las usaremos como atributos en la programación.  
En la programación los atributos se pueden definir de varias maneras:
private -> solo la clase puede ver el atributo. Para acceder a un atributo accederemos con un método que sirve para definir o hacer operaciones.
public  -> cualquier clase puede ver ese atributo.

##### Ejemplo
```java
public class Persona {
  private String nombre;
  private String apellidos;
  private String dni;
  private int numeroTelefono;
  
  public String getNombre(){
    return this.nombre;
  }
  public void getNombre(String nombreNuevo){
    this.nombre=nombreNuevo;
  }
  
  public Persona(){
    
  }
  
  public Persona(String nombre,String apellidos,String dni,int numero){
    this.nombre=nombre;
    this.apellidos=apellidos;
    this.dni=dni;
    this.numeroTelefono=numero
  }
  
}
```

Como podemos ver en el ejemplo, persona es el objeto, y como podemos fijarnos el objeto se inicializa como una clase, un objeto es una clase la diferencia que utilizaremos en java será que un objeto se intenta reconstruir un objeto con sus caracteristicas y una clase no es preciso que defina un objeto, simplemente se puede utilizar para realizar operaciones.

Los atributos delante como podemos ver llevan siempre un indicador(String-> conjunto de caracteres, int-> numeros enteros, double-> numeros decimales, boolean-> verdadero o falso) y para interactuar con ellos como podemos ver utilizaremos los métodos que lo podemos ver abajo. estos dos métodos como podemos ver hacen referéncia a nombre, el primero llamado getNombre, que nos devuelve el nombre que tenga dicha persona que se este utilizando en ese momento y lo devuelve en return, y setNombre lo que hace es modificar el valor del atributo y como podemos ver dentro del parentesis hay un valor que sera el nuevo valor del atributo, en este caso al nombre.  

Para dar los datos de los atributos podemos ir uno a uno con los setters de cada atributo pero hay una forma que se utiliza que se pondran automaticamente. Ahi es cuando aparecen lo que hemos definido como (public Persona(){}), este que tenemos aquí crearia una persona sin ninguna información, lo que deberemos hacer es pasarle los datos dentro del parentesis y después indicar donde van puesto cada valor. El this.atributo se utiliza para definir que es el atributo del objeto porque si solo pusiesemos el nombre del atributo iria al valor mas cerca y entre parentesis podemos poner el mismo nombre.
