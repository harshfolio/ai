---
tags:
  - type/prompt
  - topic/prompt-engineering
  - topic/video-generation
---

[]()# Video From Reference Image

```
{
  "reference_image": "provided",
  "video_duration": "8 seconds",
  "framerate": "30 fps",
  "camera": {
    "angle": "eye-level, slight low tilt (2–5 degrees)",
    "focal_length": "85–105 mm equivalent",
    "aperture": "f/4",
    "focus_mode": "manual, locked on the upper half of the bottle",
    "depth_of_field": "shallow with smooth background bokeh",
    "movement": [
      "linear zoom-in from full bottle frame towards the upper half over 3 seconds"
    ],
    "stabilization": "tripod or motorized slider for smoothness"
  },
  "product_movement": {
    "rotation": "none, no rotation of bottle during shot"
  },
  "background": {
    "style": "seamless solid color",
    "color": "warm beige gradient",
    "props": []
  },
  "lighting": {
    "setup": "1 key light at a 45-degree angle, 1 rim light from behind, and a soft fill light underneath",
    "brightness": "bright, soft with no overexposure",
    "shadows": "minimal soft shadows beneath bottle",
    "highlights": "subtle glossy reflections on bottle contours"
  },
  "style": {
    "mood": "clinical, premium, dermatologist-trusted",
    "color_grade": "warm bottle hues against cool background tones",
    "sharpness": "extremely high for detailed product textures"
  },
  "transitions": {
    "start": "fade in from white over 0.5 seconds",
    "end": "hold final framing, no fade out"
  },
  "text_overlay": {
    "enabled": false
  },
  "postprocessing": {
    "retouching": "flawless, no dust or imperfections",
    "color_matching": "accurate to reference",
    "resolution": "minimum 1920x1080, preferably 4K"
  },
  "audio": {
    "ambient": "subtle studio white noise, low volume throughout",
    "motion_sound": "gentle whoosh sweep for zoom, soft click when hand interacts with bottle",
    "end_accent": "very soft single chime at final framing hold",
    "volume_balance": "all sounds subtle and unobtrusive"
  },
  "scene_context": {
    "context_1": "The bottle is placed in a clinical, premium environment to highlight its quality and dermatologist-trusted status.",
    "context_2": "The camera zooms in to focus on the upper half of the bottle, emphasizing the logo and cap details.",
    "context_3": "A hand enters the frame, nudges the bottle gently (without any drastic motion), then leaves the frame.",
    "context_4": "The shot ends with the bottle remaining steady and in frame, ensuring no sudden or excessive motion. The focus remains on the product’s quality."
  }
}
```
```