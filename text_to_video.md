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
<video width="640" height="480" controls>
  <source src="images/wan21_t2v_bear.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

### Modelscope (1.7B)

