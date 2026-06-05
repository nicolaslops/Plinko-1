# PLINKO-1

## Sobre o Projeto

Este projeto consiste em uma simulação física interativa inspirada no clássico jogo mecânico **Plinko** (frequentemente associado também ao Tabuleiro de Galton). A aplicação foi estruturada utilizando HTML, CSS e o ecossistema gráfico do **p5.js**, trazendo o motor físico **Matter.js** para gerenciar a gravidade, colisões circulares, elasticidade e a aleatoriedade estatística das partículas em tempo real.

O funcionamento do cenário baseia-se em soltar pequenas partículas esféricas dinâmicas do topo da tela. À medida que caem sob o efeito da gravidade, elas colidem de forma elástica com uma grade de pinos fixos (obstáculos circulares estáticos). Essas colisões sucessivas alteram a trajetória original da partícula, fazendo-a ricochetear aleatoriamente para a esquerda ou para a direita até atingir a base, que é dividida em diferentes compartimentos de pontuação.

---

## Funcionalidades

* Geração contínua ou disparada de partículas dinâmicas com física circular realista (`Particle.js`).
* Grade de pinos estáticos dispostos estrategicamente para criar colisões procedurais (`Plinko.js`).
* Divisórias fixas na parte inferior do canvas para segmentar e agrupar as partículas caídas (`divisions.js`).
* Simulação precisa de gravidade, fricção e coeficiente de restituição (elasticidade) via `Matter.js`.
* Distribuição de probabilidade natural gerada na base através do acúmulo visual das partículas após os ricochetes.

---

## Tecnologias Utilizadas

* **HTML5**
* **CSS3**
* **p5.js** (e extensões: p5.dom, p5.play, p5.sound)
* **Matter.js** (Engine de física 2D)

---

## Objetivo

O principal objetivo deste projeto é explorar os conceitos de probabilidade e física combinatória aplicados ao desenvolvimento de jogos, simulando o efeito do Tabuleiro de Galton. O foco prático está em gerenciar um grande volume de corpos rígidos simultâneos na engine física, além de utilizar a Programação Orientada a Objetos (POO) para renderizar e estruturar os pinos, divisórias e partículas de forma limpa.

---

## Aprendizados

Durante o desenvolvimento deste projeto, foram aplicados conceitos como:

* Utilização de laços de repetição aninhados (`for`) para criar padrões e matrizes geométricas de pinos fixos no canvas.
* Programação Orientada a Objetos para a criação e controle das classes modulares `Particle.js`, `Plinko.js` e `divisions.js`.
* Calibração fina de atrito (`friction`) e elasticidade (`restitution`) para garantir que os ricochetes das esferas pareçam naturais e fluidos.
* Gerenciamento de arrays dinâmicos em JavaScript para armazenar, atualizar e desenhar múltiplas partículas em tempo real dentro do loop `draw()`.
* Organização arquitetural de diretórios isolando dependências e motores externos na pasta `libraries/`.

---

## Como Executar

1. Clone este repositório:
```bash
git clone [https://github.com/seu-usuario/PLINKO-1.git](https://github.com/seu-usuario/PLINKO-1.git)
```

2. Acesse a pasta do projeto:

```bash
cd PLINKO-1
```

3. Abra o arquivo index.html em seu navegador de preferência para observar ou interagir com a queda e os ricochetes das partículas no tabuleiro.

---

## Estrutura do Projeto
```text
PLINKO-1/
│
├── libraries/
│   ├── matter.js
│   ├── p5.dom.min.js
│   ├── p5.js
│   ├── p5.play.js
│   └── p5.sound.min.js
│
├── scripts/
│   ├── divisions.js
│   ├── ground.js
│   ├── Particle.js
│   ├── Plinko.js
│   └── sketch.js
│
├── style/
│   └── style.css
│
├── index.html
└── README.md
```

## Licença

Este projeto foi desenvolvido exclusivamente para fins educacionais e de aprendizado.

Desenvolvido como prática de desenvolvimento web e simulações matemáticas/físicas, recriando o funcionamento mecânico do Plinko através de colisões e gravidade com p5.js e Matter.js.
