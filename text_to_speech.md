## Text to Speech (Audio) 

### Speech-T5

text 
```
The dominant sequence transduction models are based on complex recurrent or convolutional 
neural networks in an encoder and decoder configuration. The best performing models also 
connect the encoder and decoder through an attention mechanism. We propose a new simple 
network architecture, the Transformer, based solely on attention mechanisms, 
dispensing with recurrence and convolutions entirely. 
```

Generated audio

https://github.com/user-attachments/assets/29e6b385-3681-4d00-9611-179faedf974a



### VITS model (MMS-TTS) 

This model series [support over 1000 languages](https://huggingface.co/facebook/mms-tts)       
English model: facebook/mms-tts-eng 

text
```
The dominant sequence transduction models are based on complex recurrent or convolutional 
neural networks in an encoder and decoder configuration. The best performing models also 
connect the encoder and decoder through an attention mechanism. We propose a new simple 
network architecture, the Transformer, based solely on attention mechanisms, 
dispensing with recurrence and convolutions entirely. 
```

https://github.com/user-attachments/assets/ed4832ac-8aa8-4477-a9a6-8dbeba3f8687


### Kokoro TTS 
Very slim model (82M)
Language code
🇺🇸 'a' => American English, 🇬🇧 'b' => British English
🇪🇸 'e' => Spanish es
🇫🇷 'f' => French fr-fr
🇮🇳 'h' => Hindi hi
🇮🇹 'i' => Italian it
🇯🇵 'j' => Japanese: pip install misaki[ja]
🇧🇷 'p' => Brazilian Portuguese pt-br
🇨🇳 'z' => Mandarin Chinese: pip install misaki[zh]

Load English pipeline
```
pipeline = KPipeline(lang_code='a')
```

text
```
The dominant sequence transduction models are based on complex recurrent or convolutional 
neural networks in an encoder and decoder configuration. The best performing models also 
connect the encoder and decoder through an attention mechanism. We propose a new simple 
network architecture, the Transformer, based solely on attention mechanisms, 
dispensing with recurrence and convolutions entirely. 
```
Generated audio

https://github.com/user-attachments/assets/886e7e0c-2eaf-4985-9aeb-900d7d795764


Load Chinese pipeline
```
pipeline = KPipeline(lang_code='z')
```

text 
```
锦瑟无端五十弦  一弦一柱思华年  庄生晓梦迷蝴蝶  望帝春心托杜鹃  沧海月明珠有泪  蓝田日暖玉生烟  此情可待成追忆  只是当时已惘然
```
Generated audio

https://github.com/user-attachments/assets/291625d4-4a0f-49aa-9959-3dc9f978c76c



### Music generation 

Model: facebook/musicgen-small 

Prompt = "classical music with violin in Bach style"

Generated audio

https://github.com/user-attachments/assets/c66dcd4c-555b-411e-9874-6518b2958422



### Voice cloning 
Model: Coqui TTS (XTTS v2)

Load model
```
tts = TTS("tts_models/multilingual/multi-dataset/xtts_v2", 
          ).to("cuda")
```

text (English)
```
The dominant sequence transduction models are based on complex recurrent or convolutional neural networks in an encoder and decoder configuration. The best performing models also connect the encoder and decoder through an attention mechanism. We propose a new simple network architecture, the Transformer, based solely on attention mechanisms, dispensing with recurrence and convolutions entirely. 
```
Generated audio

https://github.com/user-attachments/assets/aed5b38f-c2dc-4b75-ad68-6946f468cdb8


text
```
锦瑟无端五十弦，一弦一柱思华年,
庄生晓梦迷蝴蝶，望帝春心托杜鹃
沧海月明珠有泪，蓝田日暖玉生烟
此情可待成追忆，只是当时已惘然
```
Generated audio

https://github.com/user-attachments/assets/4a869f1f-87f9-45d9-a978-87b766d059e8
















