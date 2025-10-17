1) Se pueden identificar dos clases, las que son: CarroCompra que representa la clase principal que gestiona la información 
   de los productos y calcula el total de la compra. Y la segunda clase que es Calculadora representa el lado matemático que
   se utiliza para obtener el cálculo del subtotal.

   El contexto podría ser que se simula una compra, que tiene el registro de productos por su cantidad y precio en un carrito
   de compras. Se utiliza la calculadora para obtener el subtotal de cada producto, y así luego calcular el total de la compra.

2) Analizando tanto los atributos como los métodos para identificar el tipo de relación que existe entre estas clases, pude identificar
   que existe una relación de Dependencia entre CarroCompra y Calculadora, esto ya que en el método de CarroCompra llamado "subTotal"
   se crea una instancia de Calculadora para realizar la multiplicación. De esto se puede concluir que la Calculadora existe solo de
   forma temporal dentro del método y ya está.

   Es un proceso de compra gestionado por la clase CarroCompra. La clase mantiene una lista fija de 5 productos y tiene métodos para
   calcular y mostrar el total de la compra. Además, para obtener el subtotal de cada producto (cant. de productos por precio) el
   CarroCompra utiliza la clase Calculadora, que se instancia en un corto periodo de tiempo con la cantidad y el precio para realizar
   la multiplicación y obtener el costo individual, y finalmente sumarlo al costo total.
