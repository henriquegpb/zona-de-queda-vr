# Zona de Queda VR

Jogo de tiro em realidade virtual feito para o Meta Quest, rodando direto no navegador.

Você é um soldado que desembarca de uma nave no meio de uma guerra, num planeta de floresta. Do pouso em diante, precisa segurar a posição numa clareira contra ondas de drones inimigos que saem da mata.

## Como jogar

- Atire no botão **SALTAR** para começar a descida.
- Quando a luz da nave ficar verde, a batalha começa.
- Segure o gatilho para atirar e desvie dos tiros vermelhos mexendo o corpo.
- Cada onda derrotada recupera 20 de vida. A partir da onda 3 aparecem drones maiores e mais resistentes.

## Medidor de calor

O fuzil esquenta a cada tiro. A barra em cima da arma vai de verde para amarelo e depois vermelho.
Se passar de 100%, a arma **trava** até esfriar por completo. Atire em rajadas curtas.

## Controles

| Ação | Quest | PC |
|------|-------|----|
| Mirar | Controle direito | Mouse |
| Atirar | Gatilho direito | Clique |

## Como rodar

**No Quest:**
1. Abra o link do projeto no navegador do Quest.
2. Clique no botão de VR no canto inferior direito.

**No PC (para testar):**
```bash
npx serve .
```
Depois abra `http://localhost:3000` no navegador.

> O WebXR só funciona em HTTPS ou localhost. Abrir o arquivo direto pelo explorador não entra em VR.

## Tecnologias

- [A-Frame](https://aframe.io) 1.7 com WebXR
- Three.js (vem com o A-Frame)
- Web Audio API para os efeitos sonoros e o som espacial

## Estrutura

```
index.html   # jogo inteiro: cena, lógica e sons
```
