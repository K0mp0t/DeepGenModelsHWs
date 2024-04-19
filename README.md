# ДЗ 4. Обучение Stable diffusion 1.5 методом Dreambooth

## Сбор датасета для персонажа

Собрал и подготовил 26 изображений

![instance_image0](instance_images/1.jpg)
![instance_image1](instance_images/2.jpg)
![instance_image2](instance_images/3.jpg)

## Обучение Stable Diffusion 1.5

Вышло довольно неплохо, на персонажа довольно похоже

![base_street](report_images/base_model/768x1024/street.png)
![base_football](report_images/base_model/768x1024/football.jpg)

## Обучение LoRA

Поэксперементировал я много. Ниже представленны некоторые из экспериментов. Для всех экспериментов есть результаты генерации в ./report_images

### Rank=64, lr=2e-4, batch_size=3

![r64_football](report_images/lora_r64/768x1024/football.jpg)
![r64_forest](report_images/lora_r64/768x1024/forest.jpg)

### Rank=8, lr=5e-4, batch_size=3

![r8_street](report_images/lora_r8/768x1024/street.jpg)
![r8_forest](report_images/lora_r8/768x1024/forest.jpg)

## ControlNet

### Stable Diffusion 1.5

![base_monalisa](report_images/base_model/768x1024/monalisa.png)
![base_poses](report_images/base_model/768x1024/poses.png)

### LoRA Rank=64

![r64_monalisa](report_images/lora_r64/768x1024/monalisa.png)
![r64_poses](report_images/lora_r64/768x1024/poses.png)
