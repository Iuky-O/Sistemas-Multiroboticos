# Sistemas Multirobóticos
O repositório conta com cinco (5) atividades desenvolvidas ao decorrer da matéria Sistemas Multirobóticos. Para a execução das atividades foi utilizado o simulador CoppeliaSim Edu V.4.6.0 e linguagem Lua.

Site CoppeliaSim: <https://www.coppeliarobotics.com/>

## ATV 01 
Nesta atividade foi utilizado o robô Pioneer presente no simulador, este robô foi modificado e agora conta com oito (8) sensores de proximidade equipados na frente do robô.

* **Objetivo:** O objetivo é fazê-lo chegar no final idependente de onde ele saia (verde -  esquerda e vermelho - direita) em menos de cinco (5) minutos.
* **Obstáculos:** Quando for 1 está livre e números menores demostram o grau de distância do obstáculo.

Para isso, o código se desenvolveu utilizando seis (6) sensores frontais, que seguem o seguinte:

**Frente:** Segue em frente quando não tem obstáculo para os dois sensores centrais (1).

**Direita:** Vai para a direita quando a soma dos sensores 1 e 3 da esquerda forem menores do que a soma dos sensores 1 e 3 da direita. 

**Esquerda:** Vai para a esquerda quando a soma dos sensores 1 e 3 da direita forem menores do que a soma dos sensores 1 e 3 da esquerda.

**Ré:** Há duas rés, um para direita e outra para a esquerda, vai para a direita quando as distâncias 1 ou 2 direitas forem menores que _0.2_ e o mesmo acontece para a esquerda so que com as dintâncias 1 ou 2 esquerdas.

**Giro:** O robô gira quando está encurralado.


![ATV01](https://github.com/user-attachments/assets/46e32d60-5b18-46ed-8460-465aa015821e)

## ATV 02

Assim como o anterior a atividade 02 deve encontrar um caminho para o fim, agora com um robô maior e um local menor, o Robotnik tem que desviar dos obestáculos até a saída. Contando com quatro (4) sensores, codificado para ir para a frente, trás, direita e esquerda.

* **Objetivo:** Chegar até o fim do labirinto.
*  **Obstáculo:** Quando for 1 está livre e números menores demostram o grau de distância do obstáculo.

Para seguir o robô conta com:
**Direita:** Quando o sensor esquerdo 1 for menor que o sensor direito 1.
**Esquerda:** Quando o sensor direito 1 for menor que o sensor esquerdo 1.
**Frente:** Quando os sensores da frente forem maiores ou iguais 1.
**Ré:** Quando todos os sensores forem menores 1.

![ATV02](https://github.com/user-attachments/assets/ad9f09dd-3c1b-44a4-aee2-f4c1cd9338e6)

## ATV 03

* **Objetivo:** Encontrar a linha e seguir.
*  **Obstáculo:** Detecta a linha quando o elemento dados[11] < 0.3.

![ATV03](https://github.com/user-attachments/assets/c5a3564c-1c65-44ae-88a3-c2e97e091d0c)

## ATV 04

* **Objetivo:** Seguir a linha e desviar dos obstáculos.
*  **Obstáculo:** Detecta a linha quando o elemento dados[11] < 0.3.

![ATV04](https://github.com/user-attachments/assets/c5ba1880-f2c0-49cc-8212-500ccdf9fe20)

## ATV 05

* **Objetivo:** Seguir a linha e dar uma volta em pouco tempo (tempo: 16 seg.).
*  **Obstáculo:** Detecta a linha quando o elemento dados[11] < 0.3.

![ATV05](https://github.com/user-attachments/assets/f966b5ea-a9ed-48ca-99ad-8ed7e4315075)


