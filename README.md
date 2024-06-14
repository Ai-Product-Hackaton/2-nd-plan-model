# Quick plan-B model

Download and install cog

Linux:

    sudo curl -o /usr/local/bin/cog -L "https://github.com/replicate/cog/releases/latest/download/cog_$(uname -s)_$(uname -m)"
    sudo chmod +x /usr/local/bin/cog

Mac:

    brew install cog

Download the pre-trained weights:

    cog run script/download-weights

run predictions script:

    cog predict -i image=@sofa.jpg -i prompt="a modern sofa in a contemporary living room, stylish decor"

additional parameters:
    
    prompt,
    negative_prompt,
    image,
    num_inference_steps,
    controlnet_conditioning_scale,
    width,
    height,
    guidance_scale,
    generator