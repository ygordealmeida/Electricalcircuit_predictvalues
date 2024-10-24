<h1 align="center">Utilização prática da rede neural</h1>

### Essa aba visa mostrar testes feitos utilizando componentes físicos, para tal foi utilizado:

#### Fonte de Tensão Quadrática: 0V a 3,3V, Frequência 10k Hz, duty cicle 50% --> Microcontrolador NUCLEO-F446RE;

#### Osciloscópio --> Analog Discovery 3;

#### Reistor, Indutor, Capacitor --> Variam de acordo com o teste, devem ser escolhidos valores dentro ou próximos da faixa em que o modelo é treinado.

Configura-se o MCU como a fonte quadrática que alimenta o circuito RLC, em seguida com o software Waveform é possível coletar as amostras do canal ligado ao osciloscópio, com as amostras coletadas é possível plotar a figura em um código python, realizar o pré-processamento e envia-la a rede neural.


