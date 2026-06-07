# Camera

A **Camera** é o objeto que controla o ponto de vista do jogador no mundo 3D.

## Acesso

```lua
local camera = workspace.CurrentCamera
```

`CurrentCamera` é a câmera ativa no momento — é sempre assim que você a acessa via código.

## Propriedades úteis

- `CFrame` — posição e rotação da câmera no mundo
- `FieldOfView` — campo de visão em graus
- `CameraType` — define se a câmera é controlada pelo Roblox ou customizada (`Enum.CameraType.Scriptable`)

## Uso em FPS

Em jogos FPS, o [[ViewModel]] (arma + braços) é **parented diretamente à Camera**, fazendo com que ele sempre acompanhe o ponto de vista do jogador.
