
<div align="center">
  
# Multimodal LLM Study: Comprehensive Generative Suite

</div>

This repository is an all-in-one suite for open-source state-of-the-art **Multimodal Large Language Models**. It demonstrates examples for multimodal content generation by MMLLM across multiple mediums, including **text, images, video, and audio**. By leveraging cutting-edge architectures like Diffusion Transformers and Latent Consistency Models, this suite enables developers to build sophisticated generative workflows with minimal setup.

---

## 🚀 Text-to-Image (T2I)
Generate high-fidelity visual art and photorealistic images from natural language descriptions. 
* **Open-source Models:** Qwen-Image, SDXL, SD-1.5, Kandinsky 
* **Key Features:** negative prompting, LoRA weights, and control net

[Click here](text_to_image.md) to view configurations and examples

## 🚀 Image-to-Image (I2I)
Transform existing images into new styles or modify specific elements while maintaining structural integrity.
* **Open-source Models:** Qwen-Image-Edit, SDXL, RealVisXL_V4.0, controlnet-depth-sdxl-1.0-small, autoencoderKL vae: sdxl-vae-fp16-fix, 
* **Key Features:** negative prompting, inpainting, outpainting, masking, style tranfer/IP-adapter including face adapter, T2I adapter, control net, depth-map guided generation

[Click here](image-to-image.md) to view configurations and examples 

## 🚀 Text-to-Video (T2V)
Convert descriptive prompts into dynamic, high-definition video clips with consistent temporal coherence.
* **Open-source Models:** Wan-2.1, modelscope, LTX-video, AnimateDiff motion adapter 
* **Key Features:** frame rate control, and resolution scaling.

[Click here](text_to_video.md) to view configurations and examples 

## 🚀 Image-to-Video (I2V)
Animate static images into 3–5 second cinematic clips using advanced optical flow estimation.
* **Open-source Models:** SVD-img2vid-xt
* **Key Features:** keyframe animation

[Click here](image_to_video.md) to view configurations and examples 

## 🚀 Text-to-Audio (T2A)
Generate high-quality sound effects, ambient soundscapes, or musical compositions from text.
* **Open-source Models:** SVD-img2vid-xt
* **Key Features:** keyframe animation
  
* **Supported Models:** AudioLDM, MusicLM, and Bark.
* **Key Features:** Stereo output, duration control, and multi-instrumental synthesis.

[Click here](text_to_speech.md) to view configurations and examples 

---

### 📄 License
This project is licensed under the **MIT License** - see the `LICENSE` file for details.
