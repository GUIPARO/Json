# Json (JavaScript Object Notation)

Fundamentos & Estructura Json

##¿Que es un Json?
Es un formato para el intercambios de datos, básicamente **JSON** describe los datos con una sintaxis dedicada que se usa para identificar 
y gestionar los datos. **JSON** nació como una alternativa a XML, el fácil uso en javascript ha generado un gran numero de seguidores 
de esta alternativa. Una de las mayores ventajas que tiene el uso de **JSON** es que puede ser leído por cualquier lenguaje de programación. 
Por lo tanto, puede ser usado para el intercambio de información entre distintas tecnologías.

###Ejemplo:
Imaginemos que tenemos una frutería  y que queremos obtener el nombre y la cantidad de fruta y verdura que tenemos. 
En un principio vamos a suponer que tenemos lo siguiente:

##### Fruta:
* 10 manzanas
* 20 Peras
* 30 Naranjas

##### Verduras:

* 80 lechugas
* 15 tomates
* 50 pepinos

Para poder comenzar tenemos que conocer la sintaxis del **Json**

##Nombre y Valores
Para asignar a un nombre un valor debemos usar los dos puntos ‘:’ este separador es el equivalente al igual (‘=’) de cualquier lenguaje.

```json
"Nombre" : "Ivan Hdez"
```

###Valores Json
Los tipos de valores que podemos encontrar en Json son los siguientes:

* Un número **(entero o float)**
* Un string **(entre comillas simples)**
* Un booleano **(true o false)**
* Un array **(entre corchetes [] )**
* Un objeto **(entre llaves {})**
* Null

###Objetos Json
Los objetos JSON se identifican entre llaves, un objeto puede ser en nuestro caso una fruta o una verdura.
```json
{ "NombreFruta":"Manzana" , "Cantidad":20 }
```

###Array Json
En un Json puedes incluir arrays, para ellos el contenido del array debe ir entre corchetes []:
```json
{
  "Frutas": [
    {
      "NombreFruta": "Manzana",
      "cantidad": 10
    },
    {
      "NombreFruta": "Pera",
      "cantidad": 20
    },
    {
      "NombreFruta": "Naranja",
      "cantidad": 30
    }
  ]
}
```

Una vez explicado el funcionamiento de la sintaxis **JSON**, vamos a aplicar nuestro ejemplo de la frutería.
```json
{"Fruteria":
 [
  {"Fruta":
   [
    {"Nombre":"Manzana","Cantidad":10},
    {"Nombre":"Pera","Cantidad":20},
    {"Nombre":"Naranja","Cantidad":30}
   ]
  },
  {"Verdura":
   [
    {"Nombre":"Lechuga","Cantidad":80},
    {"Nombre":"Tomate","Cantidad":15},
    {"Nombre":"Pepino","Cantidad":50}
   ]
  }
 ]
}
```
Como podemos observar, hemos creado un objeto llamado frutería y, dentro de ese objeto hemos almacenado un **array de dos elementos**:

1. El primer elemento del array contiene un **objeto llamado fruta**.

2. El segundo elemento del array contiene un **objeto llamado verdura**.

Estos objetos a su vez contienen un array cuyo contenido es el **nombre** y la **cantidad** de cada fruta o verdura.

A continuacion una imagen que nos ayudara un poco a entender sobre lo que es un **JSON Object** & **JSON Array**
![GitHub Logo](http://www.androidhive.info/wp-content/uploads/2012/01/json_structor.png)

##Herramientas de visualización
Existen herramientas que nos ayudan a poder ver de manera mas estructurada nuestro **JSON**:
* [Json Viewer](http://jsonviewer.stack.hu/)
* [Json Generator](http://www.json-generator.com/)




