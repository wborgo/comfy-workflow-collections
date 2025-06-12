# Workflow: Wan Self Forcing + VACE

![Generated Video Preview](./assets/preview.gif)

![ComfyUI Workflow Preview](./assets/comfyUI.png)


This workflow uses a model derived from Wan2.1 with the **Self Forcing** technique, integrated into the video generation pipeline **VACE (Video Autoencoding via Composition and Editing)**.

The main focus here is performance: generating short videos with high visual quality, even on modest local setups.

---

## ▶️ How to Use

1. Download the workflow (.json)
2. Load the workflow into ComfyUI.
3. Provide:
   - A **reference video** (motion/animation)
   - A **reference image** (character, face, etc.)
   - Positive Prompt
4. (Optional) Apply LoRAs to add artistic style.
5. Run the pipeline.

> ⚠️ Important: The KSampler uses LCM, so the **negative prompt must be left blank**.

---

## 📌 Technical Details

- Current resolution: **480p** (e.g., 832x480)
- Duration: approximately **5 seconds**
- Frame rate: **16fps**
- Average generation time: **~2 minutes** on modest hardware

---

## 🎨 Customization

- Change the Depth Map method as desired.
- Swap the reference image for different characters.
- Apply LoRAs to add artistic style or unique visual identity to the video.

> 💡 If the reference image doesn't seem to influence the result, it's likely the background wasn't removed properly. Try using a transparent-background image (alpha channel, saved as `.png`).
