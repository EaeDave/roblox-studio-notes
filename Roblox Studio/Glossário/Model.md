# Model

Um **Model** é um container de objetos no Roblox, usado para agrupar partes relacionadas em uma única unidade.

## Características

- Herda de [[Instance]]
- Pode conter [[BasePart|Parts]], outros Models, scripts, e qualquer outro objeto
- Tem uma propriedade `PrimaryPart` que define a parte principal para posicionamento

## Uso comum

- Personagens do jogo são Models
- Armas, veículos, cenários — qualquer conjunto de objetos agrupados
- Em padrões FPS, o [[ViewModel]] é um Model parented à [[Camera]]
