## Text to Video 

This work is performed on RTX 3090 GPU (24GB)

### Wan-2.1 (14B)

Load model in 4-bit quantization 
```
pipeline_quant_config = PipelineQuantizationConfig(
  quant_backend="bitsandbytes_4bit",
  quant_kwargs={"load_in_4bit": True},
  components_to_quantize=["transformer", "text_encoder", "vae"]
)
```
Negative_prompt
```
Bright tones, overexposed, static, blurred details, subtitles, style, works, paintings, images, static, overall gray, worst quality, 
low quality, JPEG compression residue, ugly, incomplete, extra fingers, poorly drawn hands, poorly drawn faces, deformed, disfigured, 
misshapen limbs, fused fingers, still picture, messy background, three legs, many people in the background, walking backwards
```
Prompt 
```
The camera rushes from far to near in a low-angle shot, 
revealing a white ferret on a log. It plays, leaps into the water, and emerges, as the camera zooms in 
for a close-up. Water splashes berry bushes nearby, while moss, snow, and leaves blanket the ground. 
Birch trees and a light blue sky frame the scene, with ferns in the foreground. Side lighting casts dynamic 
shadows and warm highlights. Medium composition, front view, low angle, with depth of field.
```

https://github.com/user-attachments/assets/41add3a3-903f-4fe9-97b9-59d3ce9f9fc1

### Modelscope (1.7B)

Negative_prompt 
```
worst quality, inconsistent motion, blurry, jittery, distorted
```
Prompt 
```
The camera rushes from far to near in a low-angle shot, 
revealing a white ferret on a log. It plays, leaps into the water, and emerges, as the camera zooms in 
for a close-up. Water splashes berry bushes nearby, while moss, snow, and leaves blanket the ground. 
Birch trees and a light blue sky frame the scene, with ferns in the foreground. Side lighting casts dynamic 
shadows and warm highlights. Medium composition, front view, low angle, with depth of field.
```

https://github.com/user-attachments/assets/b4b61405-ecbd-4a94-aa88-b7ac4f0044d1

### LTX-Video (1.7B)

Negative_prompt 
```
worst quality, inconsistent motion, blurry, jittery, distorted
```
Prompt 
```
The camera rushes from far to near in a low-angle shot, 
revealing a white ferret on a log. It plays, leaps into the water, and emerges, as the camera zooms in 
for a close-up. Water splashes berry bushes nearby, while moss, snow, and leaves blanket the ground. 
Birch trees and a light blue sky frame the scene, with ferns in the foreground. Side lighting casts dynamic 
shadows and warm highlights. Medium composition, front view, low angle, with depth of field.
```

https://github.com/user-attachments/assets/eeb5b543-70d7-424c-a329-263dbd3e0dbb

## AnimateDiff motion adapter 

Adapter: guoyww/animatediff-motion-adapter-v1-5-2
T2V model: emilianJR/epiCRealism

Negative_prompt 
```
worst quality, inconsistent motion, blurry, jittery, distorted
```
Prompt 
```
The camera rushes from far to near in a low-angle shot, 
revealing a white ferret on a log. It plays, leaps into the water, and emerges, as the camera zooms in 
for a close-up. Water splashes berry bushes nearby, while moss, snow, and leaves blanket the ground. 
Birch trees and a light blue sky frame the scene, with ferns in the foreground. Side lighting casts dynamic 
shadows and warm highlights. Medium composition, front view, low angle, with depth of field.
```

https://github.com/user-attachments/assets/d7d229a8-9a16-4c36-82a8-0e054cc775ad


