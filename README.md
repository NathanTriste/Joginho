 (cd "$(git rev-parse --show-toplevel)" && printf '%s' 'diff --git a/README.md b/README.md
index e69de29bb2d1d6434b8b29ae775ad8c2e48c5391..afb4ca30bca2d79a1301d7306aed45b35a62464e 100644
--- a/README.md
+++ b/README.md
@@ -0,0 +1,49 @@
+# SWORD DUEL 2D
+
+Um duelo local para dois jogadores, desenhado inteiramente em Canvas e inspirado em arenas medievais indie. Sem imagens, frameworks, servidor ou dependências: abra o arquivo e lute.
+
+## Funcionalidades
+
+- Duelo simultâneo no mesmo teclado, com movimento suave, colisões, dash e stamina.
+- Ataques em arco, combo de três golpes, defesa, **Perfect Parry** e especial carregado por acertos.
+- Melhor de cinco rodadas, cronômetro, morte súbita, placar e relatório final de combate.
+- Três arenas simétricas: **Castle**, **Forest** e **Ruins**.
+- Itens aleatórios de vida, stamina e poder; partículas, impacto, screen shake e áudio Web Audio gerado no navegador.
+- Menus completos para personagem, mapa, pausa, controles, instruções, configurações e estatísticas persistentes via `localStorage`.
+
+## Controles
+
+| Ação | Player 1 — Blue Knight | Player 2 — Red Knight |
+| --- | --- | --- |
+| Movimento | W / A / S / D | Setas direcionais |
+| Ataque | F | K |
+| Defesa | G | L |
+| Dash | H | Ç |
+| Especial | R | O |
+| Pausa | ESC | ESC |
+
+O terceiro ataque consecutivo causa mais dano. Inicie a defesa pouco antes de receber um golpe para atordoar o adversário com Perfect Parry.
+
+## Tecnologias
+
+- HTML5
+- CSS3
+- JavaScript puro (Canvas 2D, Web Audio API e `localStorage`)
+
+## Como executar
+
+Baixe ou clone este repositório e abra `index.html` em um navegador moderno. Não há processo de build, backend nem instalação de pacotes.
+
+## GitHub Pages
+
+1. Envie os arquivos para um repositório GitHub.
+2. Abra **Settings → Pages** no repositório.
+3. Em **Build and deployment**, selecione **Deploy from a branch**, a branch desejada e a pasta `/(root)`.
+4. Salve e abra a URL publicada pelo GitHub. O jogo funciona como site estático.
+
+## Futuras atualizações
+
+- Novos personagens e armas.
+- Multiplayer online e ranking online.
+- Novos mapas, perigos ambientais e modo torneio.
+- IA para partidas solo e modos de treino.
' | git apply --3way)