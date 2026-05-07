# Controle de Velocidade de Motor DC com PWM utilizando NodeMCU e L293D

## Índice

1. [Introdução ao PWM](#introdução-ao-pwm)
2. [Componentes necessários](#componentes-necessários)
3. [Esquemático](#esquemático)
4. [Instruções de montagem](#instruções-de-montagem)
5. [Funcionamento do projeto](#funcionamento-do-projeto)

# Introdução ao PWM

PWM (Pulse Width Modulation), ou Modulação por Largura de Pulso, é uma técnica utilizada para controlar a potência entregue a dispositivos eletrônicos através da variação do tempo em que o sinal permanece ligado e desligado.
Neste projeto, o PWM foi utilizado para controlar a velocidade de um motor DC utilizando o NodeMCU ESP8266 e o driver L293D.
O sistema permite aumentar gradativamente a velocidade do motor através de um botão.

# Componentes necessários

- 1 NodeMCU ESP8266
- 1 CI L293D
- 1 Motor DC
- 1 Botão push button
- 1 Resistor de 10kΩ
- 1 Fonte/Bateria 5V
- Jumpers
- Proteus
- VS Code + PlatformIO

# Esquemático

O circuito foi desenvolvido utilizando o NodeMCU ESP8266 conectado ao driver L293D.
O sinal PWM é enviado ao pino EN1 do L293D para controle da velocidade do motor.
Os pinos IN1 e IN2 controlam a direção de rotação do motor.
O botão conectado ao NodeMCU permite alternar entre diferentes níveis de velocidade.

#  Instruções de montagem
Conectar o pino D9 do NodeMCU ao pino EN1 do L293D.
Conectar o pino D8 ao IN2 do L293D.
Conectar o motor DC nos pinos OUT1 e OUT2 do L293D.
Conectar o botão ao pino D2 do NodeMCU.
Alimentar o circuito com 5V.
Compilar o código no PlatformIO.
Gerar o arquivo .hex e importar no Proteus.

# Funcionamento do projeto

O projeto controla a velocidade de um motor DC utilizando PWM.
Ao pressionar o botão, o NodeMCU altera o valor do PWM enviado ao pino, aumentando gradativamente a velocidade do motor.
Os níveis de velocidade são:
25%
50%
75%
100%


