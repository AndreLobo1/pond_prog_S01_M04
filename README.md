Atividade ponderada semana 01, Parte 1: Blink Led Interno

<div align="center">
<sub>Figura 01 - Screenshot do código</sub>
<img src="/assets/screenshot.png" width="100%">
<sup>Fonte: Material produzido pelo autor (2024)</sup>
</div>

<div align="center">
<sub>Gif 01 - Arduino realizando blink</sub>
<img src="/assets/videoFuncionando.gif" width="20%">
<sup>Fonte: Material produzido pelo autor (2024)</sup>
</div>

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

