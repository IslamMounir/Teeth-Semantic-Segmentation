# Teeth-Semantic-Segmentation

This project aims to segment teeth in dental X-Rayes images using a semantic segmentation model. The model is trained on dental X-Rayes dataset. The objective is to accurately segment the teeth within the X-Rayes images.

## Dataset

The dataset consists of teeth axial view images, containing masks of the teeth. All the teeth have been grouped into a single classification named "teeth".

Here are some sample images from the dataset:

<br/>
<div align="center">
  <img src="https://github.com/IslamMounir/Teeth-Semantic-Segmentation/blob/main/images/dataset_1.jpg" alt="Dataset Sample 1" width="200"/>
  <img src="https://github.com/IslamMounir/Teeth-Semantic-Segmentation/blob/main/images/dataset_2.jpg" alt="Dataset Sample 2" width="200"/>
  <img src="https://github.com/IslamMounir/Teeth-Semantic-Segmentation/blob/main/images/dataset_3.jpg" alt="Dataset Sample 3" width="200"/>
  <img src="https://github.com/IslamMounir/Teeth-Semantic-Segmentation/blob/main/images/dataset_4.jpg" alt="Dataset Sample 4" width="200"/>
</div>

## Model Training

The semantic segmentation model is trained using the U-Net model architecture.
The model is trained to accurately segment the teeth within the axial view images. 
The training is performed for multiple epochs using the "train" dataset and was evaluated on the "valid" dataset.
The trained model evaluation results are as follows:
- Accuracy: 99.51 %
- Dice Score: 0.95


## Inference

The model was used to perform inference on a set of test images. Here are some sample ground truth masks along with the predicted masks:

  <br/>
<div align="center">
  <img src="https://github.com/IslamMounir/Teeth-Semantic-Segmentation/blob/main/images/ground_truth.jpg" alt="Inference Sample 1" width="800"/>
  <img src="https://github.com/IslamMounir/Teeth-Semantic-Segmentation/blob/main/images/pred.jpg" alt="Inference Sample 2" width="800"/>
</div>

## Usage

To use this project, follow these steps:

1. Clone the repository to your local machine.

2. Open the `train.ipynb` notebook.

3. Run the notebook to perform training, testing and inference. The notebook contains all the necessary code and instructions for each step.

4. Make sure to modify any relevant file paths or configurations within the notebook to suit your specific setup and requirements.

Feel free to explore and customize the code within the notebook to further adapt it for your needs.


## Acknowledgments

- The U-Net model architecture implementation is from this [Repo](https://github.com/aladdinpersson/Machine-Learning-Collection/tree/master/ML/Pytorch/image_segmentation/semantic_segmentation_unet).
- The dataset used in this project was collected from a publicly available source. [Click here](https://universe.roboflow.com/fathi/teeth-pwgso) to access the dataset.

