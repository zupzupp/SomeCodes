// This code is made for my first test of .NET (It's made in Visual Studio 2022, it's a console program C# (.NET framework) )


using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Proyecto_Catalina_Perez
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Bienvenid@ a \"Almacenes Por Ahí\" ^^");
            // Declaramos el total de la compra (Que al inicio es 0)
            int total = 0;
            // Declaramos los nombres de los empleados que pueden ingresar al sistema.
            List<string> nombres_empleados = new List<string>();
                nombres_empleados.Add("Catalina");
                nombres_empleados.Add("Benjamín");
                nombres_empleados.Add("Beyoncé");
                nombres_empleados.Add("A");

            Console.WriteLine("Ingrese su nombre para validación");

           string nombre = Console.ReadLine();

            // Si el nombre concuerda, lo dejamos comprar.
            if (nombres_empleados[0] == nombre || nombres_empleados[1] == nombre || nombres_empleados[2] == nombre || nombres_empleados[3] == nombre)
            {
                Console.WriteLine("Bienvenid@ " + nombre);

                // Creamos las listas de los nombres de los productos, los precios de los productos y la boleta
                // que es la que tendrá los datos de nuestra compra.
                List <string> nombres_productos = new List<string>();
                List<int> precio_productos = new List<int>();
                List<string> boleta = new List<string>();

                // Añadimos los nombres a nombres_productos.
                nombres_productos.Add("Camisas");
                nombres_productos.Add("Pantalones");
                nombres_productos.Add("Polerones");

                // Añadimos los precios de los productos (en el mismo orden que ingresamos los nombres).
                precio_productos.Add(15000);
                precio_productos.Add(20000);
                precio_productos.Add(10000);

                // Iniciamos un bucle para que se repita hasta que el vendedor quiera dejar de ingresar datos.
                while(true) 
                    {
                    // Presentamos los productos y las opciones.
                    Console.WriteLine("Ingrese el elemento que comprará");
                    Console.WriteLine("1. Camisas ($15.000)");
                    Console.WriteLine("2. Pantalones ($20.000)");
                    Console.WriteLine("3. Polerones ($10.000)");
                    Console.WriteLine("4. Imprimir boleta");
                    Console.WriteLine("5. Salir");

                    // Consultamos la elección y la transformamos a entero.
                    Console.WriteLine("\nIngrese su elección: ");
                    int seleccion = Convert.ToInt32(Console.ReadLine());

                    // Con un switch vemos la opción que eligió el vendedor.
                    switch (seleccion)
                    {
                        // Comprar camisas a $15000
                        case 1:
                            Console.WriteLine("Elegiste camisas");
                            total += precio_productos[0];
                            boleta.Add(nombres_productos[0]);
                            Console.WriteLine("Total: ${0}", total);
                            break;

                        // Comprar pantalones a $20000
                        case 2:
                            Console.WriteLine("Elegiste pantalones");
                            total += precio_productos[1];
                            boleta.Add(nombres_productos[1]);
                            Console.WriteLine("Total: ${0}", total);
                            break;

                        // Comprar polerones a $10000
                        case 3:
                            Console.WriteLine("Elegiste polerones");
                            total += precio_productos[2];
                            boleta.Add(nombres_productos[2]);
                            Console.WriteLine("Total: ${0}", total);
                            break;

                        // Imprimir boleta
                        case 4:
                            Console.WriteLine("***BOLETA***");
                            Console.WriteLine("Productos seleccionados:");
                            foreach (string producto in boleta)
                            {
                                Console.WriteLine("-" + producto);
                            }
                            Console.WriteLine("Total a pagar: ${0}", total);
                            Console.WriteLine(" ");
                            break;

                        // Salir de la aplicación
                        case 5:
                            Console.WriteLine("Gracias por comprar, vuelva pronto ^^ ");
                            Console.ReadKey();
                            return;

                        // En caso de que no haya ingresado ninguna opción válida, lo hacemos que ingrese la opción nuevamente.
                        default:
                            Console.WriteLine("Opcion inválida. Por favor, elija nuevamente.");
                            break;
                    }
                }
            }

            // Si no concuerda, no lo dejamos ingresar.
            else
            {
                Console.WriteLine("Tu nombre no esta registrado");
                Console.ReadKey();
                return;
            }


        }
    }
}   
