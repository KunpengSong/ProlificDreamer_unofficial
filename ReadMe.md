# Unofficial implementation of ProlificDreamer. 

This is a third party implementation of the paper:"[ProlificDreamer: High-Fidelity and Diverse Text-to-3D
Generation with Variational Score Distillation](https://arxiv.org/abs/2305.16213)". 

The code is largely built on a combination of [stable-dreamfusion](https://github.com/ashawkey/stable-dreamfusion) and [stable-diffusion-LoRA](https://huggingface.co/docs/diffusers/v0.13.0/en/training/lora)

Starting from stable-dreamfusion, I:
- added stable-diffusion LoRA module
- added MLP to UNet to take in camera perspective as additinal input
- achieved improved results in text-to-3D than Dreamfusion

To Do list:
- add timestep annealing
- scale up resolution
- add image-to-3D

To use the code:
- install requirements as instructed on the [stable-dreamfusion](https://github.com/ashawkey/stable-dreamfusion) and [stable-diffusion-LoRA](https://huggingface.co/docs/diffusers/v0.13.0/en/training/lora) page
- use the .sh file as extrance: sh run_1.sh
