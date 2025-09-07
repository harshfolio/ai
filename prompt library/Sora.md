---
tags:
  - type/prompt
  - topic/prompt-engineering
  - topic/image-generation
---

# Professional Product Image from low-res product image with white background

```
{
  "reference_image": "provided",
  "product": {
    "description": "White pump bottle with soft green label featuring 'Clinikally' branding and 'HydraSoft Gentle Skin Cleanser' text, along with the details: 'Hydrating', 'Enriched with Glycerin, Vitamin B3 and B5', 'For Dry to Sensitive Skin', and '125 ml'.",
    "reference_match": "color, shape, label, and logo must exactly match reference image"
  },
  "shot": {
    "type": "close-up macro",
    "angle": "slight low angle or straight-on with slight tilt for depth",
    "framing": "tight on the upper half or full label, leaving subtle breathing space",
    "focus": "pin-sharp on label text and texture details",
    "depth_of_field": "shallow, with smooth bokeh in background"
  },
  "background": {
    "style": "ultra-clean studio",
    "color": "pure white or subtle warm gradient",
    "props": []
  },
  "lighting": {
    "setup": "multi-point studio with softboxes",
    "quality": "high key lighting with controlled shadows",
    "brightness": "very bright with no overexposure",
    "reflections": "carefully placed highlights to emphasize gloss and shape contours",
    "accent_light": "optional rim light for subtle edge separation"
  },
  "style": {
    "mood": "luxury skincare ad, clinical but aspirational",
    "texture": "highlight micro-texture of bottle and label",
    "color_grade": "neutral, true-to-life with clean whites",
    "sharpness": "extremely high, suitable for print-quality ad"
  },
  "postprocessing": {
    "retouching": "perfectly clean, remove dust and blemishes",
    "color_correction": "match reference image",
    "output_resolution": "very high (minimum 4k)",
    "consistency": "professional product ad quality"
  },
  "text_overlay": {
    "enabled": false
  }
}

```