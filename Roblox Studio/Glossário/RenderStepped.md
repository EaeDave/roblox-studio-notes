# RenderStepped

**RenderStepped** é um evento do serviço `RunService` que dispara a cada frame, **antes** da renderização da cena.

## Acesso

```lua
local RunService = game:GetService("RunService")

RunService.RenderStepped:Connect(function(deltaTime)
    -- código executado todo frame
end)
```

- `deltaTime` — tempo em segundos desde o último frame

## Quando usar

- Atualizar a posição do [[ViewModel]] para seguir a [[Camera]]
- Animações visuais que precisam ser suaves
- Qualquer coisa que precise rodar no lado do **cliente** a cada frame

## Atenção

- Só funciona no **cliente** (LocalScript) — não existe no servidor
- Usar código pesado aqui pode causar queda de FPS
- Para lógica que não precisa rodar antes da renderização, prefira `Heartbeat`
