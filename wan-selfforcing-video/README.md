# Workflow: Wan Self Forcing + VACE

Este workflow usa o modelo derivado do Wan2.1 com a técnica **Self Forcing**, integrado ao pipeline de geração de vídeo **VACE (Video Autoencoding via Composition and Editing)**.

O foco aqui é performance: geração de vídeos curtos com alta qualidade visual, mesmo em setups locais modestos.

---

## ⚙️ Requisitos

- **GPU**: RTX 3060 (mínimo 12GB VRAM)
- **RAM**: 16GB
- [ComfyUI instalado](https://github.com/comfyanonymous/ComfyUI)
- Modelos necessários:
  - `wan-sf-1.3b` (modelo Self Forcing)
  - Depth detector (Canny / OpenPose / Midas, etc.)
  - Background remover (ex: MODNet)
  - Modelo LoRA (opcional)

---

## ▶️ Como usar

1. Carregue o `workflow.json` no ComfyUI.
2. Insira:
   - Um **vídeo de referência** (animação/movimento)
   - Uma **imagem de referência** (personagem, rosto, etc.)
3. (Opcional) Aplique LoRAs para adicionar estilo artístico.
4. Execute o pipeline.

---

## 📌 Detalhes técnicos

- Resolução atual: **480p**
- Duração: até **5 segundos**
- Frame rate: **16fps**
- Tempo médio de geração: **~2 minutos** em hardware modesto

---

## 🎨 Personalização

- Altere o método de Depth Map conforme sua preferência.
- Troque a imagem de referência para diferentes personagens.
- Aplique LoRAs para adicionar estilo ou identidade visual ao vídeo.

---

## 🧪 Resultado

*Adicione aqui uma imagem ou link para um exemplo gerado, se quiser mostrar o impacto visual do pipeline.*

---
