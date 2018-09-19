# clases-c-
link github del profe: https://github.com/utec-cs1100/cpp
https://www.greenteapress.com/thinkcpp/thinkCScpp.pdf 
www.rankred.com/useful-c-cheat-sheets/ 
Temas hasta el primer hackerrank : bucles y funciones
----------------------------------------------------------------------------

Ejercicio: de radianes a sexagesimales

#include <iostream>
#include <cmath>  //el valor de pi en cmath es M_PI

using namespace std;

int main()
{
    float a = 0;
    cin >> a;
    cout << (a*180)/M_PI;
}
--------------------------------------------------------------------------------

#include <iostream>
#include <cmath>  //tai loy

using namespace std;

int main()
{
   int x;
   cin>>x;
   int a = x/24;
   int resto = x%24;
   int b = resto/12;
   int resto2 = resto%12;
   int c = resto2/6;
   int resto3 = resto2%6;
   cout << a<<'\n'<<b<<'\n'<<c<<'\n'<<resto;

}
---------------------------------------------------------------------------------
miercoles 29 de agosto 2018
---------------------------------------------------------------------------------

Ejercicio: hallar distancia entre dos puntos

#include <iostream>
#include <cmath>

using namespace std;

int main()
{
     double distancia;
     int xm, ym ;
     int x1, y1, x2, y2;

    cin >> x1 >> y1;
    cin >> x2 >> y2;

    distancia = sqrt(pow(x2-x1,2) + pow(y2-y1,2));

    /*
    cout << "xm:"<< xm << "\n";
    cout << "ym:"<< ym << "\n";
    *\
    cout << "distancia:"<< distancia ;

}

-----------------------------------------------------------------------------------

Ejercicio: sumar dos angulos sexagesimales (2do lab ejercicio2)

#include <cmath>

using namespace std;

int main()
{
    int G1, M1, S1, G2, M2, S2;
    int b, c;

    cin >> G1>>M1>>S1;
    cin >> G2>>M2>>S2;

    int r = (S1 +S2)%60;
    int llevo = (int) (S1 +S2)/60;
    b = M1 + M2 + llevo;
    int llevo2 = (int)(b/60);
    b = b%60 ;
    c = G1 + G2 + llevo2;

    cout << c << ' '<< b <<' '<< r << '\n';
}

-----------------------------------------------------------------------------------

Ejercicio: repetir letra por cada nro

#include <iostream>                 
#include <cmath>

using namespace std;

int main()
{
    int nro,i = 0;
    string letra;
    cin >> nro >> letra;

    do
    {
        cout << letra << '\n';
        i++;
    }
    while ( i < nro );

}

-------------------------------------------------------------------------------------
miercoles 05 de septiembre 2018
-------------------------------------------------------------------------------------

Ejercicio: 1,2,3,4 otño, ....

#include <iostream>
using namespace std;

int main() 
{
  int n;
  cin >> n;
  
  if (1<= n <=4)
  {
    switch (n)
    {
      case 1 : cout << "Otoño"<< endl;
                    break;
      case 2 : cout << "Invierno"<< endl;
                    break;
      case 3 : cout << "Primavera"<< endl;
                    break;
      case 4 : cout << "Verano"<< endl;
      
    }
  }
}

----------------------------------------------------------------------------------------

Ejercicio: un programa que lea nros hasta 0

#include <iostream>
using namespace std;

int main()
{
  int cn=0, cp=0, cimp=0;
  int x = -1;
  while (x!=0)
  {
      cout << "Ingrese un nro: "<< endl;
      cin >> x;
      if (x!=0)
      {
          cn++;
          if (x%2==0)
          {
             cp++;
          }
          else
          {
             cimp++;
          }
      }
      
      cout << "cn: "<< cn << "cp: "<< cp << "cimp: "<< cimp << endl;
  }
}  

------------------------------------------------------------------------------------
viernes 7 de agosto 2018
------------------------------------------------------------------------------------
 ejercicio: sumar del 1 al 100
 
 #include <iostream>
#include <cmath>

using namespace std;

int main()
{
    int i = 0;
    int s = 0;
    for(i=1;i<=100;i++)
    {
        s+=i;
    }
    cout<<s<<endl;
}

---------------------------------------------------------------------------------------
 
ejercicio : suma de cuadrados con nros de inicio y fin

#include <iostream>
#include <cmath>

using namespace std;

int main()
{
    int a,b;
    cin >> a >> b;

    if (a % 2 !=0)
        a++;
    if (b % 2 !=0)
        b--;
    int s = 0;
    while (a<=b){
        s = s + pow(a,2);
        a+=2;
    }
    cout << s <<;
}

-----------------------------------------------------------------------------------------

ejercicio: Sumatoria de factoriales desde 1 hasta un número ingresado por el teclado entre 1 y 15. Usando do while.

#include <iostream>
#include <cmath>

using namespace std;

int main()
{
    int x;
    cin >> x;
    int s = 0;
    int n = 1;
    do {
        auto producto = 1;
        for (int i = 1; i <= n; i++)
            producto = producto * i;
        s += producto;
        producto = 1;
        n++;
    } while (n <= x);
    cout << "suma de factoriales:" << s;

}

----------------------------------------------------------------------------------------------

ejercicio: contador de nros, pares e impares hasta que se introduzca 0.

#include <iostream>
#include <cmath>

using namespace std;

int main()
{
    int x = 1;
    int cn = 0, cp=0, cimp=0;   //contador nros pares e impares.

    while (x !=0)
    {
      cin >> x;
      if (x!=0)
      {
          cn++;
          if (x % 2 == 0)
              cp++;
          else if (x % 2 != 0)
              cimp++;
      }
    }
    cout << "nro total leídos :" <<cn<<endl;
    cout << "nros pares :" << cp<<endl;
    cout << "nros impares :" <<cimp<<endl ;

}
------------------------------------------------------------------------------------------
FALTA TERMINAR !!!!!!!!!!!

#include <iostream>
#include <cmath>

using namespace std;

int main()
{
    int palm=0, caprob=0, cjalados=0, total=0;
    int n1, n2, n3 ,n4 , n5 ;
    int n;

    cin >>n;
    int i = 1;
    
    while (i++<=n)
    {
        cout<< "Ingrese notas del alumno(a)" << i <<endl;
        cin>>n1>>n2>>n3>>n4>>n5;
        palm = (n1+n2+n3+n4+n5)/5;
        if (palm>10.5)
            caprob++;
        else
            cjalados++;
        total += palm;

    }
    int promtotal= total/n;
    cout << 
}

-----------------------------------------------------------------------------------------------
Ejercicio de piramides (03 lab sesion 1)

#include <iostream>

using namespace std;

int main()
{
    int i, n, valor;

    cout << "introduzca valor  :" << endl;
    cin >> valor;
    cout << endl;

    if (valor > 1, valor < 21)
    {
        for (i = 1; i <= valor; i++)
        {
            for (n = 1; i >= n; n++)
                cout << "*";
            cout << "\n";
        }
     }
}

------------------------------------------------------------------------------------------------
Ejercicio : convertir nro de cualquier base a base 10 (03 lab sesion 1)

#include <iostream>

using namespace std;

int main()
{
    int numero; //a convertir
    int base; //base en que estaexpresado
    int resultado; //ovbio
    int resto; //resto de division
    int potencia; // valor por el que se multiplica cada cifra
            printf("numero y base?");
    scanf("%d", &numero);
    scanf("%d", &base);
    //compruebo que está entre 2 y 10
    if (base < 2 , base > 10){
        printf("BASE INCORRECTA");
        exit(0);
    }
    potencia = 1;
    resultado = 0;
    do{
        resto = numero %10;
        numero = numero / 10;
        resultado = resultado + (resto * potencia);
        potencia = potencia * base;
    } while (numero =! 0);
    printf("resultado = %d ", resultado);
}
-------------------------------------------------------------------------------------------------
viernes 14 de septiembre 2018  Día del repaso para el hackerrank
-------------------------------------------------------------------------------------------------
ejercicios de bucles 1 (02 lab sesion 2) 
#include <iostream>   

using namespace std;

int main()
{
    int N, s =0;
    cin >> N;
9
    for (int i=1; i<=N; i++)
    {
        if (i%2==0)
        {
          s+=i;
        }
    }
    cout << s << endl;
}
---------------------------------------------------------------------------------------------------
ejercicios de bucles 3:la mayor potencia de 2 menor o igual a N (02 lab sesion 2 )

#include <iostream>  
#include <cmath>

using namespace std;

int main ()
{
    int N;
    cin >>N;
    int potencia = 2;
    while (potencia <= N)
    {
        potencia *=2 ;
    }
   cout<<potencia/2<<endl;
}

 ----------------------------------------------------------------------------------------------------
otra forma de hacer el de mayor potencia con for

#include <iostream> 
using namespace std;

int main ()
{
    int N;
    cin >>N;
    int potencia = 2;
    for (int i = 1; potencia<N;i++)
    {
        potencia *=2 ;
    }
   
   cout<<potencia/2<<endl;
}
contest de hoy
https://www.hackerrank.com/contests/sp0-poo1/challenges
--------------------------------------------------------------------------------------------------------
#include <iostream>

using namespace std;

int sumaDigitos(int Num) {
    int Suma = 0, Resto;

    while (Num != 0) {
        Resto = (Num % 10);
        Suma = (Suma + Resto);
        Num = (Num / 10);
    }
    return (Suma);
}
int main()
{
    int N, s, r;
    cin>>N;

    if (N>1)
    {
        cout<<sumaDigitos(N);
    }
}
