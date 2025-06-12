# Workflow: Wan Self Forcing + VACE

Este workflow usa o modelo derivado do Wan2.1 com a técnica **Self Forcing**, integrado ao pipeline de geração de vídeo **VACE (Video Autoencoding via Composition and Editing)**.

O foco aqui é performance: geração de vídeos curtos com alta qualidade visual, mesmo em setups locais modestos.

---


## ▶️ Como usar

1. Baixe o workflow (.json)
2. Carregue o workflow no ComfyUI.
3. Insira:
   - Um **vídeo de referência** (animação/movimento)
   - Uma **imagem de referência** (personagem, rosto, etc.)
   - Prompt Positivo
4. (Opcional) Aplique LoRAs para adicionar estilo artístico.
5. Execute o pipeline.

Importante: O KSample utiliza LCM, logo, o prompt negativo deve ser mantido em branco

---

## 📌 Detalhes técnicos

- Resolução atual: **480p** (exemplo: 832x480)
- Duração: aproximadamente **5 segundos**
- Frame rate: **16fps**
- Tempo médio de geração: **~2 minutos** em hardware modesto

---

## 🎨 Personalização

- Altere o método de Depth Map conforme sua preferência.
- Troque a imagem de referência para diferentes personagens
- Aplique LoRAs para adicionar estilo ou identidade visual ao vídeo.

Caso a imagem de referência não esteja sendo levada em consideração, provavelmente o modelo não removeu seu fundo corretamente, tente com uma imagem sem fundo originalmente (canal alpha transparente, salvo como .png)


