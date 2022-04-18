# productsList
Lista de productos con base de datos local realizado en el segundo trimestre del segundo año de DAM

# Conceptos de Android
Los métodos OnCreate que aparece en cada clase al inicio, son métodos que crean la pantalla cuando se va a acceder a ella así como todas las propiedades necesarias para ello.

El método OnResume es el encargado de, al "minimizar" la aplicación, cuando se vuelve a la aplicación, que aparezca por donde estaba.

Las interfaces/vistas se hacen mediante archivos xml donde aparece la pantalla y se puede añadir todos los elementos que se requiera. Cada elemento debe tener constrains para anclarlos a la pantalla y que no le afecte si el dispositivo es más grande o más pequeño. También se puede ver el código del mismo.

Cada clase Java de la vista está conectada al xml mediante el ID del xml. Es decir, se referencia al xml.

Ejemplo:

variable = findViewById(R.id.archivo_xml)

Lo mismo se aplica para conectar los elementos de la clase con la vista xml.

## En el caso de los RecyclerView
Los RecyclerView no son más que listas de tarjetas que se van a mostrar en la pantalla. Cada item de esa vista, cada objeto tiene una serie de datos y, para ello, también hay que hacer referencia. Para ello, se hace igual pero indicando mediante el "itemview" que entra por parametro.

Ejemplo: 

public Holder(@NonNull View itemView) {

            super(itemView);
            variable = itemView.findViewById(R.id.elemento_xml);
            
        }
        
El itemview del parametro es lo que va a indicar que el cambio que se haga solo va a afectar a ese item y no a todos los items de la lista.


