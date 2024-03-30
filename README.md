// https://www.tinkercad.com/things/a8UpwVhmxuj-codigo-morse

// Vamos enviar a mensagem TADS em Codigo Morse.
// Traço " - " 3 unidades de tempo HIGH = 3000 delay.
// Bolinha " • " 1 unidade de tempo HIGH = 1000 delay.
// Espaço entre partes da mesma letra 1 unidade de tempo LOW = 1000 delay.
// Espaço entre letras 3 unidades de tempo LOW = 3000 delay.

int LED = 2;

void setup() {
  pinMode(LED, OUTPUT);
}

void loop() {
  // T = -
  digitalWrite(LED, HIGH);
  delay(3000);
  digitalWrite(LED, LOW);
  delay(3000);
  
  // A = •-
  digitalWrite(LED, HIGH);
  delay(1000);
  digitalWrite(LED, LOW);
  delay(1000);
  digitalWrite(LED, HIGH);
  delay(3000);
  digitalWrite(LED, LOW);
  delay(3000);
  
  // D = -••
  digitalWrite(LED, HIGH);
  delay(3000);
  digitalWrite(LED, LOW);
  delay(1000);
  digitalWrite(LED, HIGH);
  delay(1000);
  digitalWrite(LED, LOW);
  delay(1000);
  digitalWrite(LED, HIGH);
  delay(1000);
  digitalWrite(LED, LOW);
  delay(3000);
  
  // S = •••
  digitalWrite(LED, HIGH);
  delay(1000);
  digitalWrite(LED, LOW);
  delay(1000);
  digitalWrite(LED, HIGH);
  delay(1000);
  digitalWrite(LED, LOW);
  delay(1000);
  digitalWrite(LED, HIGH);
  delay(1000);
  digitalWrite(LED, LOW);
  delay(3000);
}
