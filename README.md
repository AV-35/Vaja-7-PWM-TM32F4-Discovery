# Vaja 7 - krmiljenje PWM signala

## Cilj naloge

S pomočjo programskega okolja STM32CubeIDE in HAL knjižnicami sprogramirajte mikroprocesor tako, da boste generirali PWM signal in ga tudi krmilili na izbranem izhodu STM32F4 Discovery. Za preizkus potrebujete osciloskop.

## Postopek inicializacije periferije

- pini za vhode sje **PE9**.  
- Poleg pina se izpiše **TIM1_CH1**.  
- Vrednost Prescalerja je **16**.  
- sedaj znaša **100kHz**
- Ta parameter spreminja moč signala.
- *sConfigOC.Pulse = x;*
- *sConfigOC.Pulse = 25;*
- Ukazi:
  <ol type=1>
  <li>Pošlje signal na pin</li>
  <li>Poveča dutyCycle za 10</li>
  <li>Previri če je dutyCycle nad 90 in ga spremeni na 10 ce je</li>
  </ol>

## Slika osiloskopa 25%
![25](media/SDS00001.BMP)
## Slika osiloskopa 50%
![25](media/SDS00002.BMP)
## Slika osiloskopa 100%
![25](media/SDS00003.BMP)

## Pinout/Configuracija

<p align="center">
<img src="media/Pinout.png">
</p>

<p align="center">
<img src="media/Connfig_1.png">
</p>

<p align="center">
<img src="media/Connfig_2.png">
</p>

## Vezje
<p align="center">
<img src="media/Vezje.png">
</p>

## Komentar 
Koda deluje brezhibno.


