# water_plastic_pollution_detector

 This project identifies polluted and clean water > 

![image](https://github.com/user-attachments/assets/c402dd72-e17a-44fd-9ef6-6dbe91687b66)



## The Algorithm

 
The algorithm works by running all the pictures in it's collection of images to identify certain features that would be used to classify the selected image as clean or polluted. Images include but are not limited to the following:
![clean_water37](https://github.com/user-attachments/assets/ff7a2321-b977-4c0d-919b-c7f108e26965)
![igaveuponnames](https://github.com/user-attachments/assets/40d0cabf-c700-47ab-af32-41bc20b7c0d0)
![erhgsouehgbeou](https://github.com/user-attachments/assets/0f23d25d-a52f-4f54-a5bf-d24742ec272f)


## Running this project

  # Make sure that you are out of the docker
  Use [ls models/water_plastic_pollution_detector/] to make sure that the model is on the nano. You should see a file called resnet18.onnx.
  # Set the NET and DATASET variables
  
[NET=models/water_plastic_pollution_detector]

[DATASET=data/water_plastic_pollution_detector]

Run this command to see how it operates on an image from the clean_water folder.

imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/clean_water4.jpg clean_water.jpg

# open VS code to see the image output

