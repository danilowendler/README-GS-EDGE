# Sistema de Monitoramento da Qualidade da Água

## 🗒️ Autores
- Danilo Wendler - RM: 556602
- Pedro Muzel - RM: 555983
- Lucas Raphael - RM: 555543

## 📁 Link para o Projeto no Tinkercad
[Projeto no Tinkercad](https://www.tinkercad.com/things/gkts8yF8ZMk-projeto-gs-edge)

## 🗒️ Descrição do Projeto
Este projeto utiliza um Arduino Uno para monitorar a qualidade da água através de sensores de temperatura, pH e turbidez, exibindo os dados coletados em um display LCD 16x2. O projeto foi desenvolvido para alertar e informar sobre a saúde dos oceanos e a poluição da água.

## 🗒️ Objetivo
O objetivo deste projeto é criar um sistema que permita monitorar parâmetros críticos da qualidade da água, proporcionando uma maneira simples e eficaz de visualizar esses dados em tempo real.

## 🗒️ Componentes Necessários
- Arduino Uno
- Sensor de temperatura (LM35)
- Potenciômetro 10kΩ (para ajuste do contraste do LCD)
- Dois potenciômetros adicionais (para simular sensores de pH e turbidez)
- Display LCD 16x2
- Resistor 220Ω (opcional, usado apenas em hardware real)
- Breadboard
- Fios de conexão

## 🛠️ Montagem do Circuito
### 🛠️ Sensor de Temperatura (LM35)
- Conecte o pino de saída do LM35 ao pino A0 do Arduino.
- Conecte o pino VCC do LM35 ao 5V do Arduino.
- Conecte o pino GND do LM35 ao GND do Arduino.

### 🛠️ Potenciômetros (para simular sensores de pH e turbidez)
- **Potenciômetro para pH:**
  - Conecte o terminal central ao pino A1 do Arduino.
  - Conecte um dos terminais laterais ao 5V.
  - Conecte o outro terminal lateral ao GND.
- **Potenciômetro para turbidez:**
  - Conecte o terminal central ao pino A2 do Arduino.
  - Conecte um dos terminais laterais ao 5V.
  - Conecte o outro terminal lateral ao GND.

### 🛠️ Display LCD 16x2
- Conecte o pino VCC do LCD ao 5V do Arduino.
- Conecte o pino GND do LCD ao GND do Arduino.
- Conecte o pino Vo ao cursor central do potenciômetro de 10kΩ (os outros dois terminais do potenciômetro ao 5V e GND).
- Conecte o pino RS ao pino 7 do Arduino.
- Conecte o pino E ao pino 8 do Arduino.
- Conecte os pinos D4, D5, D6, D7 aos pinos 9, 10, 11, 12 do Arduino, respectivamente.

## 🛠️ Código Arduino
O código estará presente no vídeo apresentado.

## 🛠️ Instruções de Uso
### Montagem do Circuito:
1. Monte o circuito conforme descrito na seção "Montagem do Circuito".
2. Certifique-se de que todas as conexões estejam firmes e corretas.

### 🛠️ Carregar o Código no Arduino:
1. Conecte o Arduino ao computador através do cabo USB.
2. Abra o Arduino IDE.
3. Copie e cole o código fornecido na seção "Código Arduino" no editor do Arduino IDE.
4. Selecione a porta correta e o modelo do Arduino (Arduino Uno).
5. Carregue o código no Arduino.

### 🗒️ Executar o Projeto:
1. Após carregar o código, o LCD deverá inicializar e exibir "Qualidade da Agua".
2. O sistema começará a exibir as leituras de temperatura, pH e turbidez no LCD.

### 🗒️ Ajuste de Parâmetros:
- Utilize os potenciómetros para ajustar e simular as leituras dos sensores de pH e turbidez.
- O potenciômetro de 10kΩ ajusta o contraste do LCD para melhor visualização.

## 🗒️ Requisitos
### Hardware:
- Arduino Uno
- Componentes listados na seção "Componentes Necessários"

## 🗒️ Dependências
- Biblioteca LiquidCrystal (incluída na instalação padrão do Arduino IDE)

## Considerações Finais
Este projeto é uma implementação básica para monitorar a qualidade da água usando sensores simulados. Em uma aplicação real, sensores específicos de pH e turbidez seriam utilizados para obter dados precisos. O projeto pode ser estendido para incluir conectividade com a Internet das Coisas (IoT) para monitoramento remoto e alertas em tempo real.
