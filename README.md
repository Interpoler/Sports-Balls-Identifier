## Sports Balls Identifier
My sports ball identifier can identify 12 different types of balls through image classification via imagenet
This is a showcase of my project classifying a baseball
https://imgur.com/a/v5GqdQb

## Potential Use of My Project
I can integrate my image recognizer on sports balls to a camera used for sports ball sorting. This can help speed up the sorting of balls in recreational centers also streamlining equipment management. This optimizes the efficiency of the sports center.

## The Algorithm
Image classification works by loading a pre-trained deep learning model, preprocessing the input image, and passing it through the model. The model computes probabilities for each class label, and post-processing selects the highest probability label as the prediction. I have a dataset consisting of 6000 photos of the 12 types of balls for training, I trained my model for 34 epochs so that my jetson can accurately differentiate between the 12 types of balls.

## Running this project
1. Download everything in code
2. Setup your nano to your computer hotspot's ip address
3. Connect to the ip address of the nano via vscode
4. Paste all the code into vscode
5. Type the commands below seperately

1. cd
2. cd jetson-inference/python/training/classification
3. NET=models/cat_dog
4. DATASET=data/cat_dog
5. imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/(ball you want to recognize)/(specific image)      6. (output image name)

## Video Explanantion
[View a video explanation here](video link)















# Sports-Balls-Identifier
I can integrate my image recognizer on sports balls to a camera used for sports ball sorting. This can help speed up the sorting of balls in recreational centers also streamlining equipment management. This optimizes the efficiency of the sports center.
