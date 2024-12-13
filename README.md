# styleGAN2-ADA
 Synthesizing Computerized Tomographic Medical Images using styleGAN2-ADA

### styleGAN2-ADA Original Project
![image](https://github.com/user-attachments/assets/e976675c-2125-4020-90f0-99aa03952a81)

### styleGAN2-ADA Medical Image Synthesis
![image](https://github.com/user-attachments/assets/51b0afdf-af8b-4ba1-9d93-463417861793)


# Prerequisites
<pre>
- 1–8 high-end NVIDIA GPUs with at least 12 GB of memory.
- 64-bit Python 3.7 and PyTorch 1.7.1. 
- CUDA toolkit 11.0 or later. Use at least version 11.1 if running on RTX 3090.
</pre>

# Get Started
<pre>
# Generate images without truncation 
python generate.py --outdir=out --trunc=1 --seeds=85,265,297,849 --network=.pkl    
# Generate images with truncation
python generate.py --outdir=out --trunc=0.7 --seeds=600-605 --network=.pkl
# Generate class conditional images
python generate.py --outdir=out --seeds=0-35 --class=1 --network=.pkl
# Style mixing example
python style_mixing.py --outdir=out --rows=85,100,75,458,1500 --cols=55,821,1789,293 --network=.pkl
</pre>

# References
<pre>
styleGAN2-ADA, 
paper: Karras, T., Aittala, M., Hellsten, J., Laine, S., Lehtinen, J., & Aila, T. (2020). Training generative adversarial networks with limited data. Advances in neural information processing systems, 33, 12104-12114.
URL: https://github.com/NVlabs/stylegan2-ada-pytorch.git
</pre>
