# UI (User Interface)

**UI** é o conjunto de elementos visuais 2D exibidos na tela do jogador, como botões, labels, barras de vida e menus.

## Onde fica

Os elementos de UI ficam dentro de um `ScreenGui`, que por sua vez fica em:
- `StarterGui` — no editor (é replicado para o jogador ao entrar)
- `PlayerGui` — na instância do jogador em runtime

## Elementos comuns

| Elemento | Uso |
|---|---|
| `TextLabel` | Exibir texto |
| `TextButton` | Botão clicável |
| `ImageLabel` | Exibir imagem |
| `Frame` | Container/painel |
| `[[ViewportFrame]]` | Renderizar objetos 3D dentro da UI |

## ViewportFrame

O [[ViewportFrame]] é um elemento de UI especial que consegue renderizar objetos 3D dentro de um frame 2D — útil para previews de itens, scopes de mira, etc.
