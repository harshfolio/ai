
---
tags:
  - type/prompt
  - topic/prompt-engineering
  - topic/image-generation
---


> [!NOTE] Title
> ⬆️ Upload an image you want to render with this style in ChatGPT, then paste this JSON:
> 
> ![[Pasted image 20250716221320.png]]


```

{
  "task": "Retexture an uploaded object into a hyper-realistic 3D product render",
  "user_input": {
    "uploaded_image": "<UPLOAD_IMAGE_HERE>"
  },
  "style_reference": "Photorealistic 3D product render inspired by Apple keynote visuals and 'Apple Intelligence' aesthetics — smooth materials, soft gradient backgrounds, and flawless studio lighting",
  "instructions": {
    "preserve_geometry": true,
    "retexture_object": {
      "material_preferences": {
        "main_body": "brushed aluminum or matte anodized metal",
        "accents": "semi-frosted polycarbonate or translucent acrylic",
        "buttons": "smooth tactile metal or frosted finish",
        "dials_or_controls": "textured metal with soft knurling"
      },
      "color_palette": {
        "base": "#D4D4D4",
        "accent": "#F0F0F0",
        "control_elements": "#2A2A2A",
        "highlight": "#FF3B3B"
      }
    },
    "render_settings": {
      "lighting": "Flawless studio lighting with soft shadows and diffused highlights, similar to Apple product renders",
      "background": "smooth pastel gradient (e.g., soft blush, light lavender, cloud blue, or mint green)",
      "camera_view": "same as input image",
      "aspect_ratio": "1:1",
      "resolution": "ultra high",
      "output_format": "PNG"
    },
    "additional_notes": "Maintain the original shape and camera angle of the object. Upgrade its surface texture, lighting, and background to showcase it like a premium Apple product with cinematic realism and a balanced square (1:1) composition."
  }
}
```