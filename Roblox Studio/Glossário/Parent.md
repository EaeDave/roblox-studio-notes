# Parent / Parented

No Roblox, todo objeto tem uma propriedade **Parent** que define quem é o seu "dono" na hierarquia do jogo. Dizer que um objeto está **parented** a outro significa que ele é filho desse objeto.

## Como funciona

A hierarquia do Roblox funciona como uma árvore. Um objeto só existe e é visível no jogo se estiver parented (direta ou indiretamente) ao `game` ou ao `workspace`.

```lua
local parte = Instance.new("Part")
parte.Parent = workspace -- "parenta" a parte ao workspace
```

## Exemplos

- Um `[[Model]]` parented ao `workspace` aparece no mundo 3D
- Um `ScreenGui` parented ao `PlayerGui` aparece na tela do jogador
- O `[[ViewModel]]` parented à `[[Camera]]` faz com que a arma siga o ponto de vista do jogador

## Remover do jogo

Setar `Parent` para `nil` remove o objeto do jogo (equivalente a destruí-lo temporariamente):

```lua
objeto.Parent = nil -- remove da hierarquia
objeto:Destroy()    -- remove e limpa da memória definitivamente
```
