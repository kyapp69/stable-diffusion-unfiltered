# Stable Diffusion without the safety/NSFW filter and watermarking!

This is a fork of Stable Diffusion that disables the horribly inaccurate NSFW filter and unnecessary watermarking. The goal of this is three-fold:

1. Saves precious time from images that get mistakenly censored, especially if you run this on a Colab notebook.
2. Saves GPU memory by not loading the safety models, allowing for some more headroom on GPUs with smaller VRAM.
3. Reverts the state of the Stable Diffusion scripts to the closed beta, when these weren't implemented yet.

Additionally, removing the watermark might reduce some quality loss or artifacts while using the software to generate images, although this is yet to be fully tested.

You can use this in the exact same way as the [original Stable Diffusion](https://github.com/CompVis/stable-diffusion) does.

For use in Colab notebooks that rely on the original Stable Diffusion, simply replace all instances linking to `!git clone https://github.com/CompVis/stable-diffusion.git` with `!git clone https://github.com/chemistzombie/stable-diffusion-unfiltered.git`

Disclaimer: I don't encourage or condone people to breach the [CreativeML Open RAIL-M license](https://huggingface.co/spaces/CompVis/stable-diffusion-license) used by Stable Diffusion. This repo is solely intended to address the issues with false positives that frequently occur while using the software, as well as improving usability on GPUs with smaller VRAM.