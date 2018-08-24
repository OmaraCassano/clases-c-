# clases-c-
link github del profe: https://github.com/utec-cs1100/cpp
https://www.greenteapress.com/thinkcpp/thinkCScpp.pdf 
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
-----------------------------------------------------------------------------
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


