# NumerosPrimos_GR_Flutter

NOMBRE: Guillermo Rivera

APLICACIÓN EN FLUTTER SOBRE NÚMEROS PRIMOS - CAPTURA

Para el funcionamiento de la aplicación que devuelva la cantidad de números primos es necesaria la siguiente función la cual se llama al momento de hacer
tap en el botón de la interfaz:

(No me permite adjuntar capturas, adjunto el código)

void _generatePrimO() {
    int contador = 0;
    int num = 100;
    for (var i = 1; i <= num; i++) {
      if (num % i == 0) {
        contador++;
      }
    }
    if (contador == 2) {
      setState(() {
        _a = num;
      });
    } else {
      _generatePrimO();
    }
  }
