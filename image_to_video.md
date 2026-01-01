## Image to Video

This work is performed on RTX 3090 GPU (24GB)

### SVD-img2vid-xt

load model
```
model_id = "stabilityai/stable-video-diffusion-img2vid-xt"
pipeline = StableVideoDiffusionPipeline.from_pretrained(
    model_id, 
    torch_dtype=torch.float16, 
)
```
Original image               
![pic33](images/cogvideox_rocket.png)  

Generated video      


https://github.com/user-attachments/assets/67ee972b-27a3-40d4-92a0-8cb8bf6f60b4



Original image               
![pic33](images/2026.png)  

Generated video      

https://github.com/user-attachments/assets/fdcd6a1c-d0fc-407b-ab38-b5b156fb9857

Original image               
![pic33](images/pic_33.jpg)  

Generated video      

https://github.com/user-attachments/assets/249f057b-b6db-4100-93c2-53f698678194

