# clases-c-
link github del profe: https://github.com/utec-cs1100/cpp
https://www.greenteapress.com/thinkcpp/thinkCScpp.pdf 
www.rankred.com/useful-c-cheat-sheets/ 
----------------------------------------------------------------------------

#include <iostream>
#include <cmath>  //de radianes a sexagesimales, el valor de pi en cmath es M_PI

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
hallar distancia entre dos puntos
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
sumar dos angulos sexagesimales (2do lab ejercicio2)

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

