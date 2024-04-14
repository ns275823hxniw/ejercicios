# ejercicios
ejercicio 01
int main() {
  // Get the number of chickens, cows, and pigs from the user.
  int chickens, cows, pigs;
  cout << "Enter the number of chickens: ";
  cin >> chickens;
  cout << "Enter the number of cows: ";
  cin >> cows;
  cout << "Enter the number of pigs: ";
  cin >> pigs;

  // Calculate the total number of legs for each type of animal.
  int chickenLegs = chickens * 2;
  int cowLegs = cows * 4;
  int pigLegs = pigs * 4;

  // Calculate the total number of legs for all the animals.
  int totalLegs = chickenLegs + cowLegs + pigLegs;

  // Print the total number of legs.
  cout << "The total number of legs is: " << totalLegs << endl;

  return 0;
}


    ejercicio 2
    #include <iostream>
#include <algorithm> // Incluye la biblioteca <algorithm> para usar transform

using namespace std;

int main() {
  // Variable para almacenar la entrada del usuario
  string entrada;

  // Solicitar al usuario que ingrese true o false
  cout << "Ingrese true o false: ";
  cin >> entrada;

  // Convertir la entrada a minúsculas
  transform(entrada.begin(), entrada.end(), entrada.begin(), ::tolower);

  // Invertir el valor de la entrada
  string salida;
  if (entrada == "true") {
    salida = "false";
  } else if (entrada == "false") {
    salida = "true";
  } else {
    salida = "Entrada no válida";
  }

  // Mostrar el resultado
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
ejercicio 5 #include <iostream>

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
