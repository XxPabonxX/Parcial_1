# Parcial_1

/*1)
#include<iostream>
#include<stdlib.h>

using namespace std;

int main() {
    int cont = 0, cont_mayores = 0, cont_menores = 0;
    float numero = 1, promedio_numeros = 0, promedio_mayores = 0, promedio_menores = 0, mayor_menores = 0,
        mayor_mayores = 0, vect_numeros[100]{}, vect_mayores[100]{}, vect_menores[100]{};
    
    while (numero != 0.0)
    {
        cout << "Ingrese el numero " << cont + 1 << ": ";
        cin >> numero;

        if (numero !=0.0)
        {
            vect_numeros[cont] = numero;
            cont++;
        }


    }

    system("cls");

    for (int i = 0; i < cont; i++)
    {
        promedio_numeros += vect_numeros[i];
    }

    promedio_numeros = (promedio_numeros / cont);

    for (int i = 0; i < cont; i++)
    {
        if (vect_numeros[i]>promedio_numeros)
        {
            vect_mayores[cont_mayores] = vect_numeros[i];
            cont_mayores++;
        }
        else
        {
            vect_menores[cont_menores] = vect_numeros[i];
            cont_menores++;
        }
    }

    for (int i = 0; i < cont; i++)
    {
        promedio_mayores += vect_mayores[i];
        promedio_menores += vect_menores[i];
    }

    promedio_mayores = (promedio_mayores / cont_mayores);
    promedio_menores = (promedio_menores / cont_menores);

    cout << "El vector de numeros es: ";
    for (int i = 0; i < cont; i++)
    {
        cout << vect_numeros[i] << " ";
    }

    cout << endl << "El vector de numeros mayores es: ";
    for (int i = 0; i < cont_mayores; i++)
    {
        cout << vect_mayores[i] << " ";
        if (vect_mayores[i]>mayor_mayores)
        {
            mayor_mayores = vect_mayores[i];
        }
    }

    cout << endl << "El vector de numeros menores es: ";
    for (int i = 0; i < cont_menores; i++)
    {
        cout << vect_menores[i] << " ";
        if (vect_menores[i] > mayor_menores)
        {
            mayor_menores = vect_menores[i];
        }
        
    }

    cout << endl << endl << "El promedio del vector de numeros es: " << promedio_numeros;
    cout << endl << "El promedio del vector de numeros mayores es: " << promedio_mayores;
    cout << endl << "El promedio del vector de numeros menores es: " << promedio_menores;

    if (promedio_menores>promedio_mayores)
    {
        cout << endl << "El promedio mas alto se encuentra en el vector de numeros menores de la media.";
    }
    else {
        cout << endl << "El promedio mas alto se encuentra en el vector de numeros mayores de la media.";
    }

    cout << endl << endl << "El mayor numero del vector de numeros menores de la media es: " << mayor_menores;
    cout << endl << "El mayor numero del vector de numeros mayores de la media es: " << mayor_mayores << endl;

    system("Pause");
    return 0;
}
*/

/*2)
#include<iostream>
#include<stdlib.h>

using namespace std;

int main() {

    int filas = 5, columnas = 5;

    for (int i = 0; i < filas; i++)
    {
        for (int j = 0; j < columnas; j++)
        {
            if (i == 0) {
                if (j == 0 || j == 4) {
                    cout << "1 ";
                }
                else
                {
                    cout << "0 ";
                }
            }
            if (i==1)
            {
                if (j==1 || j==3)
                {
                    cout << "0 ";
                }
                else
                {
                    cout << "2 ";
                }
            }
            if (i==2)
            {
                if (j==1)
                {
                    cout << "* ";
                }
                else if (j==3)
                {
                    cout << "0 ";
                }
                else
                {
                    cout << "3 ";
                }
            }if (i==3)
            {
                if (j==1)
                {
                    cout << "+ ";
                }
                else if (j==0 || j==2)
                {
                    cout << "4 ";
                }
                else
                {
                    cout << "0 ";
                }

                
            }if (i==4)
            {
                if (j==1)
                {
                    cout << "+ ";
                }
                else if (j==3)
                {
                    cout << "* ";
                }
                else
                {
                    cout << "5 ";
                }
            }
        }
        cout << endl;
    }
    cout << endl;
    system("Pause");
    return 0;
}
*\
