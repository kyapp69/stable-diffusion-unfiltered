# Stable Diffusion without the safety/NSFW filter and watermarking!

This is a fork of Stable Diffusion that disables the horribly inaccurate NSFW filter and unnecessary watermarking. The goal of this is three-fold:

1. Saves precious time from images that get mistakenly censored, especially if you run this on a Colab notebook.
2. Saves GPU memory by not loading the safety models, allowing for some more headroom on GPUs with smaller VRAM.
3. Reverts the state of the Stable Diffusion scripts to the closed beta, when these weren't implemented yet.

You can use this in the exact same way as the [original Stable Diffusion](https://github.com/CompVis/stable-diffusion) does.

For use in Colab notebooks that rely on the original Stable Diffusion, simply replace all instances linking to `!git clone https://github.com/CompVis/stable-diffusion.git` with `!git clone https://github.com/chemistzombie/stable-diffusion-unfiltered.git`