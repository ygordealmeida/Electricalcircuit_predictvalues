<h1 align="center">Utilização da Rede Neural em Montagens Físicas</h1>

### Essa aba visa mostrar testes feitos utilizando componentes físicos, para tal foi utilizado:

#### Fonte de Tensão Quadrática: 0V a 3,3V, Frequência 10k Hz, duty cicle 50% --> Microcontrolador NUCLEO-F446RE;

#### Osciloscópio --> Analog Discovery 3;

#### Reistor, Indutor, Capacitor --> Variam de acordo com o teste, devem ser escolhidos valores dentro ou próximos da faixa em que o modelo é treinado.

Configura-se o MCU como fonte quadrática que alimenta o circuito RLC, em seguida com o software Waveforms é possível coletar as amostras do canal ligado ao osciloscópio, a ponta de prova esta ligada de tal forma que observamos a tensão sobre o resistor, com as amostras coletadas, dividimos a tensão no resistor pelo valor da resistência que já é conhecido assim obtemos i(t), então é realizado a plotagem da figura em um código python, após isso se faz o pré-processamento e a figura é enviada para a rede neural.

#### Na execução dessa aba foi utilizado um circuito com R= 300 ohms, L = 335 µH, C = 7,57 nF 

#### Foi obtido como previsão: R= 301,729 ohms, L= 530,411 µH, C= 9,956 nF 



<div align="center">
  <img src="https://github.com/user-attachments/assets/b31fe43f-dd43-453a-adc0-752d433b60a7" alt="Circuit Image 1" width="500" style="display: inline-block;"/>
  <img src="https://github.com/user-attachments/assets/4cec2168-276e-433e-bd7b-4cd83bb8b19f" alt="Circuit Image 2" width="500" style="display: inline-block;"/>
</div>

