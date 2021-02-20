# MegaPlaza
En MegaPlaza se hace un 20% de descuento a los clientes  cuya compra supere los 300.
using System;

namespace Descuento_en_compra_mayor_a_Q300._00
{
    class Program
    {
        static void Main(string[] args)
        {
            short cantidad;
            short descuento;
            Console.Write("Buen día estimado cliente, por favor ingrese la cantidad a pagar: ");
            cantidad = Convert.ToInt16(Console.ReadLine());

            if (cantidad > 300)
            {
                descuento = (short)((cantidad * 20) / 100);
                cantidad = (short) (cantidad - descuento);
                Console.WriteLine("Usted cuenta con un 20% de descuento, su nuevo total a pagar es de Q."+cantidad);

            }else if (cantidad < 300)
            {
                Console.WriteLine("Su cantidad a pagar es de: Q."+cantidad);
            }

        }
    }
}
