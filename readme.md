# Ideogram 4: does it follow plain English? With and without LoRA
Set of experiments to see difference between ideogram fast model and with applied Ideogram4-Natural-Language-Text-Encoder

<p align="left">
<a href="https://novmikvis.github.io/ideogram-4-prompt-adherence-test/">
  <img src="https://github.com/user-attachments/assets/4a0ef548-5e1b-4166-a859-cc276e244626" width="1000" alt="mrjackspade's Natural-Language Text-Encoder LoRA">
</a>
</p>



#### **[Open the viewer →](https://novmikvis.github.io/ideogram-4-prompt-adherence-test/)**

I rendered the same 16 prompts four ways: stock Ideogram 4 with no adapter, and with [mrjackspade's Natural-Language Text-Encoder LoRA](https://huggingface.co/mrjackspade/Ideogram4-Natural-Language-Text-Encoder) at checkpoints 1000, 3010, and 5000.

That's 64 images total. Seed is the same everywhere — `424242424242` — and so is the preset: `Default 20` (20 steps, mu 0.0, std 1.75). Only the adapter changes across a row, so you see exactly what the LoRA adds.

The point is plain language. The LoRA tries to make normal descriptions work as well as structured Magic Prompt input. So no JSON, no bounding boxes, no hex lists here. Just the way people actually write: 270–600 words per prompt, with exact counts, left-to-right positions, materials, lighting, and every line of text that should appear in the image.

Prompts are diverse: text rendering, dense typography, strict palette limits, spatial relations, object catalogs, crowds, realistic skin, extreme aspect ratios, multilingual signs, charts, and comic panels.

## How to use the viewer

* Hover a thumbnail in the right rail to preview it. Click to pin it.
* Scroll to zoom, drag to pan. Zoom is shared, so the crop stays in place when you hover over variants. Zoom into small text once and compare it across all four.
* Keys: `1`–`4` switch variant, `↑` `↓` switch prompt, `p` shows the full prompt, `esc` resets zoom.

## Reproducibility

Every image has ComfyUI workflow embeded. Drag any frame into ComfyUI and you get the exact workflow
