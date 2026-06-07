# ViewModel vs ViewportFrame (FPS)

## ViewModel

- Não é uma classe nativa do Roblox — é um **padrão de design** da comunidade
- Um [[Model]] com a arma + braços, **[[Parent|parented]] à** [[Camera|CurrentCamera]]
- Totalmente **3D**, atualizado via [[RenderStepped]]
- **Padrão da indústria** em jogos FPS no Roblox

## ViewportFrame

- Classe [[UI]] nativa do Roblox
- Renderiza objetos 3D dentro de um **frame 2D** na tela
- Em FPS, usado em contextos secundários: mira telescópica (scope), preview de inventário, menus de seleção de armas

## Resumo

| | ViewModel | ViewportFrame |
|---|---|---|
| Natureza | 3D (na câmera) | UI 2D que renderiza 3D internamente |
| Uso em FPS | Principal (arma na tela) | Secundário (scopes, UI) |
| Popularidade em FPS | Alta | Baixa |
