Atividade ponderada semana 01, Parte 1: Blink Led Interno

<div align="center">
<sub>Figura 01 - Screenshot do código</sub>
<img src="/assets/screenshot.png" width="100%">
<sup>Fonte: Material produzido pelo autor (2024)</sup>
</div>

<br>
<br>
<br>
<div align="center">
<img src="/assets/videoFuncionando.gif" width="20%">
</div>
<br>
<br>
<br>

Código da imagem:

```cpp
// Função setup que será executada uma vez ao pressionar o reset ou ligar a placa
void setup() {
  // inicializa o pino digital LED_BUILTIN como uma saída
  pinMode(LED_BUILTIN, OUTPUT);
}

// Função loop que será executada continuamente
void loop() {
  digitalWrite(LED_BUILTIN, HIGH);  // liga o LED (HIGH é o nível de tensão)
  delay(300);                       // espera por 300 milissegundos
  digitalWrite(LED_BUILTIN, LOW);   // desliga o LED, definindo a tensão para LOW
  delay(300);                       // espera por 300 milissegundos
}
```

Cógido da segunda parte da ponderada, simulando blink externo no tinkercad

```cpp
// Função setup que será executada uma vez ao pressionar o reset ou ligar a placa
void setup() {
  pinMode(13, OUTPUT); // Define o pino 13 como saída
  pinMode(7, OUTPUT);  // Define o pino 7 como saída
}

// Função loop que será executada continuamente piscando os leds como um pisca-pisca 
void loop() {
  digitalWrite(13, HIGH); // Liga o LED na porta 13
  digitalWrite(7, LOW);   // Desliga o LED na porta 7
  delay(300);             // Espera 300 milissegundos

  digitalWrite(13, LOW);  // Desliga o LED na porta 13
  digitalWrite(7, HIGH);  // Liga o LED na porta 7
  delay(500);             // Espera 500 milissegundos
}
```

Link do tinkercad
https://www.tinkercad.com/things/eadmueOpQzz/editel?sharecode=u9OZ-3f_WuhvDSsnH2LiNMXVDTpXnBhJr-MEm6hWZ5M
