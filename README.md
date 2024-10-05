# Awesome-Music-Generation
## Welcome to MMGen!
### Try our demo first! 
&ensp; &rarr; &ensp; 
<a href="https://awesome-mmgen.github.io/"><img src="https://img.shields.io/static/v1?label=Demo! Check out amazing results&message=MMGen&color=purple&logo=github.io"></a> &ensp; &larr; &ensp; Click here!

&ensp; &rarr; &ensp; 
<a href="https://arxiv.org/abs/2409.20196"><img src="https://img.shields.io/static/v1?label=Paper&message=arXiv.2409&color=red&logo=arXiv"></a> &ensp; &larr; &ensp; Click here!


&ensp; &rarr; &ensp; 
<a href="https://huggingface.co/ManzhenWei/MMGen"><img src="https://img.shields.io/static/v1?label=CKPT&message=huggingface&color=yellow&logo=huggingface.co"></a> &ensp; &larr; &ensp; Click here!  
This repository contains the implementation of the music generation model **MMGen**, the first novel approach using melody to guide the music generation that, despite a pretty simple method and extremely limited resources, achieves excellent performance.

Anyone can use this model to generate personalized background music for their short videos on platforms like TikTok, YouTube Shorts, and Meta Reels. Additionally, it is very cost-effective to fine-tune the model with your own private music dataset.

## Video
You can watch the introduction video on  

&ensp; &rarr; &ensp; 
<a href="https://youtu.be/kc2n-ByWB-M?si=U-gjvAuBjD-HOtS7"><img src="https://img.shields.io/static/v1?label=Watch&message=YouTube&color=red&logo=youtube"></a> &ensp; &larr; &ensp; Click here!

&ensp; &rarr; &ensp; 
<a href="https://www.bilibili.com/video/BV1K84FeBEqo/?share_source=copy_web&vd_source=d808713ed70be6b862e6ccbcb28d2f5b"><img src="https://img.shields.io/static/v1?label=Watch&message=Bilibili&color=blue&logo=bilibili"></a> &ensp; &larr; &ensp; Click here!

## Online Service

Now you can try music generation with your own prompt on our   

&ensp; &rarr; &ensp; 
<a href="https://www.mmgen.online/"><img src="https://img.shields.io/static/v1?label=Try it&message=MMGen Website&color=green&logo=googlechrome"></a> &ensp; &larr; &ensp; Click here!

**Tips**: To generate high-quality music using MMGen, you would want to craft detailed and descriptive prompts that provide rich context and specific musical elements.


## Quick Start

To get started with **MMGen**, follow the steps below:

### Step 1: Clone the repository
```bash
git clone https://github.com/shaopengw/Awesome-Music-Generation.git
cd Awesome-Music-Generation
```

### Step 2: Set up the Conda environment
```bash
# Create and activate the environment from the provided environment file
conda env create -f environment.yml
conda activate MMGen_quickstart
```

### Step 3: Download checkpoints from [huggingface](https://huggingface.co/ManzhenWei/MMGen)
```bash
# Ensure that the checkpoints are stored in the following directory structure
Awesome-Music-Generation/
└── data/
    └── checkpoints/
```

### Step 4: Modify the PYTHONPATH environment variables in the quick_start.sh script
```bash
# Update the paths to reflect your local environment setup
# Replace:
export PYTHONPATH=/mnt/sda/quick_start_demonstration/Awesome-Music-Generation:$PYTHONPATH
export PYTHONPATH=/mnt/sda/quick_start_demonstration/Awesome-Music-Generation/data:$PYTHONPATH
# With:
export PYTHONPATH=/your/local/path/Awesome-Music-Generation:$PYTHONPATH
export PYTHONPATH=/your/local/path/Awesome-Music-Generation/data:$PYTHONPATH
```

### Step 5: Assign execution permissions for the script
```bash
chmod +x quick_start.sh
```
### Step 6: Execute the quick start script
```bash
bash quick_start.sh
```
### Allow the script to run for several minutes. Upon completion, the results will be available in the following directory:
```bash
Awesome-Music-Generation/log/latent_diffusion/quick_start/quick_start
```


## Checkpoints
https://huggingface.co/ManzhenWei/MMGen

## Todo List
- [x] Demo website
- [x] Huggingface checkpoints
- [x] Quick start (Inference)
- [ ] Training Datasets
- [ ] Training/fine-tuning code
- [x] Online free generation service
- [ ] Checkpoints on larger datasets



---

Feel free to explore the repository and contribute!

## Citation

```bibtex
@article{wei2024melodyneedmusicgeneration,
      title={Melody Is All You Need For Music Generation}, 
      author={Shaopeng Wei and Manzhen Wei and Haoyu Wang and Yu Zhao and Gang Kou},
      year={2024},
      eprint={2409.20196},
      archivePrefix={arXiv},
      primaryClass={cs.SD},
      url={https://arxiv.org/abs/2409.20196}, 
}
