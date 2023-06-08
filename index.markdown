---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: "Cyclic One-Way Diffusion"
---


<img src=assets/pipeline.jpg />


## Environment Preparation:

Follow the setup of LDM repo: [LDM](https://github.com/CompVis/latent-diffusion/tree/main). Download pretrained T2I model sd-v1-4.ckpt to main folder.




## Command:

To run COW, just enter command:

```
python scripts/COWrunner.py [--outputs_folder[OUTDIR]] [--data_folder[DATADIR]] [--text_path[TEXTDIR]] 

optional arguments:
  --outputs_folder[OUTDIR]     dir to write the results to
  --data_folder[DATADIR]       dir to load the input text conditions
  --text_path[TEXTDIR]         dir to load the input visual conditions
```



the output saved every two cycles, will be in the "outputs" folder.

## Run with your own human face visual and text condition

Put your data and backgroundmask under folder "data/image". Add your own text in "data/prompt.txt", one text for a batch.