# RPS Classification

## Overview Problems
Permasalahan dari project ini yaitu bagaimana cara membuat model dengan akurasi bagus dari dataset RPS

<p>
    <img src="https://storage.googleapis.com/tfds-data/visualization/fig/rock_paper_scissors-3.0.0.png"/>
</p>

![image 1](https://storage.googleapis.com/tfds-data/visualization/fig/rock_paper_scissors-3.0.0.png)

## Overview Dataset
Dataset ini sudah tersedia pada website tensorflow, dataset dibagi menjadi 70% training, 25% validation, 5% testing.<br>link url untuk download dataset: https://storage.googleapis.com/laurencemoroney-blog.appspot.com/rps.zip

## Preprocessing and Modeling
Pada bagian preprocessing data di rescale 1/255 lalu rotasi, zoom, shear, shift dengan masing-masing 20%, random flip dan fill nearest setelah rotasi dan shift

Untuk model kami menggunakan model _MobileNet_ dan ini adalah ilustrasi bagaimana _MobileNet_ berkerja

![image 2](https://www.researchgate.net/publication/348830807/figure/fig1/AS:1022398732185600@1620770261147/Schematic-diagram-of-the-MobileNet-SSD-network-model-structure.jpg)

Summary Model:

![image 3](summary.png)

Graph accuracy dan loss model:

![image 4](graph.png)

Evaluate Model:

![image 5](result.png)

## Prediction and Deployment

Kami mengambil 10 image acak dari testing dan memperhatikan apakah model dapat memprediksi image dengan baik, berikut ini adalah hasilnya:

![image 6](predict.png)

Deployment kami menggunakan streamlit dan berikut ini contohnya:

![image 7](deploy-1.png)

![image 8](deploy-2.png)