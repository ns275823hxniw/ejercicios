# ejercicios
ejercicio 01
int main() 

{
  
  int chickens, cows, pigs;
  cout << "Enter the number of chickens: ";
  cin >> chickens;
  cout << "Enter the number of cows: ";
  cin >> cows;
  cout << "Enter the number of pigs: ";
  cin >> pigs;

 
  int chickenLegs = chickens * 2;
  int cowLegs = cows * 4;
  int pigLegs = pigs * 4;

  
  int totalLegs = chickenLegs + cowLegs + pigLegs;

  
  cout << "The total number of legs is: " << totalLegs << endl;

  return 0;
}


    ejercicio 2
    #include <iostream>
#include <algorithm> 

using namespace std;

int main() {
  
  string entrada;

  
  cout << "Ingrese true o false: ";
  cin >> entrada;

 
  transform(entrada.begin(), entrada.end(), entrada.begin(), ::tolower);

  
  string salida;
  if (entrada == "true") {
    salida = "false";
  } else if (entrada == "false") {
    salida = "true";
  } else {
    salida = "Entrada no válida";
  }

  
  cout << "Valor invertido: " << salida << endl;

  return 0;
}

ejercicio 3
#include <iostream>

using namespace std;

int convert(int hours, int minutes) {
  int seconds = (hours * 3600) + (minutes * 60);
  return seconds;
}

int main() {
  int hours, minutes;
  cout << "ingrese horas: ";
  cin >> hours;
  cout << "ingrese minutos: ";
  cin >> minutes;
  cout << "segundos: " << convert(hours, minutes) << endl;
  return 0;
} 


ejercicio 4
#include <iostream>

using namespace std;

int footballPoints(int wins, int draws, int losses) {
  return (wins * 3) + (draws * 1) + (losses * 0);
}

int main() {
  int wins, draws, losses;
  cout << "Enter the number of wins, draws, and losses: ";
  cin >> wins >> draws >> losses;
  cout << "Total points: " << footballPoints(wins, draws, losses) << endl;

  return 0;
}
ejercicio 5 

#include <iostream>
using namespace std;

int calc_age(int age) {
  return age * 365;
}

int main() {
  int age;
  cout << "introduzca su edad: ";
  cin >> age;
  cout << "tu edad en dias es: " << calc_age(age) << endl;
  return 0;
}
ejercicios c++
