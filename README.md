# Visualizing Class Activation Maps (CAM) with Different Algorithms

Welcome to the project on visualizing class activation maps (CAM) using different algorithms! In this repository, we explore various techniques to gain insights into Convolutional Neural Networks (CNNs) and understand how they make decisions on image classification tasks.

CAM is a powerful visualization technique that helps us identify the regions in an input image that significantly contribute to a model's predictions. By highlighting these important regions, we can better comprehend the CNN's decision-making process, interpret its behavior, and ensure that it focuses on relevant features during inference.

The main goal of this project is to demonstrate the effectiveness of different CAM visualization algorithms and compare their strengths and weaknesses. We will utilize the popular VGG16 model, pre-trained on the ImageNet dataset, to showcase the visualization techniques.

#  Key Differences Among the Algorithms:

|              | Grad Cam                          | Grad Cam Plus Plus                 | Score Cam                   | Faster Score Cam            |
|--------------|-----------------------------------|-----------------------------------|-----------------------------|-----------------------------|
| Algorithm    | Gradient-based                    | Gradient-based                    | Gradient-free               | Gradient-free               |
| Explanation  | Highlights important regions      | Highlights important regions      | Highlights important regions| Highlights important regions|
|              | based on gradient information    | based on gradient information    | without using gradients     | without using gradients     |
| Interpretability | Interpretable heatmaps         | Interpretable heatmaps         | Interpretable heatmaps      | Interpretable heatmaps      |
| Model Layer  | Typically uses the last          | Typically uses the last          | Can use any layer          | Can use any layer          |
|              | convolutional layer              | convolutional layer              |                             |                             |
| Tuning       | Requires tuning hyperparameters  | Requires tuning hyperparameters  | Requires minimal tuning     | Requires minimal tuning     |
| Performance  | May be computationally expensive | May be computationally expensive | Efficient                   | Efficient                   |
| Pros         | Widely used and easy to implement| Improves localization accuracy   | No gradient computation     | No gradient computation     |
|              | Good interpretability            | Better heatmaps for some models   | Less sensitive to noise     | Less sensitive to noise     |
| Cons         | Can suffer from noise            | Complexity may lead to overfitting| Less detailed heatmaps      | Less detailed heatmaps      |




**Project Structure:**
- `Visualizing_Class_Activation_Maps_CAM_with_Different_Algorithms.ipynb`: This Jupyter Notebook contains the code and step-by-step tutorial for visualizing CAM using various algorithms like Grad Cam, Grad Cam Plus Plus, Score Cam, and Faster Score Cam.
- `requirements.txt`: A text file listing the required Python packages and their versions to run the notebook code effectively.

**Getting Started:**
- Clone this repository to your local machine using Git to access all the code and data files.
- Install the required packages mentioned in the `requirements.txt` file using `pip`.
- Open the Jupyter Notebook (`Visualizing_Class_Activation_Maps_CAM_with_Different_Algorithms.ipynb`) to explore the CAM visualization algorithms and execute the code cells to see the visualizations.

**Note:**
Please ensure you have the necessary Python environment set up, including TensorFlow, Matplotlib, NumPy, and `tf-keras-vis` package, to run the code without any issues.

#  Results :
Original Images : 
<img width="415" alt="image" src="https://github.com/FarzadMalik/4_class_activation_maps_visualization_algorithms/assets/107833662/bcc91ee0-9cea-4613-9641-38b9c29f768d">


Grad CAM:
<img width="416" alt="image" src="https://github.com/FarzadMalik/4_class_activation_maps_visualization_algorithms/assets/107833662/7dff0d2b-74a6-4391-9015-fcd1e0309401">


GradCAM++:
<img width="416" alt="image" src="https://github.com/FarzadMalik/4_class_activation_maps_visualization_algorithms/assets/107833662/51c431c0-761d-4653-baf4-203e38853e25">

ScoreCAM:
<img width="416" alt="image" src="https://github.com/FarzadMalik/4_class_activation_maps_visualization_algorithms/assets/107833662/47459740-e50d-46ba-8ae2-113b32868016">


Faster ScoreCAM:
<img width="415" alt="image" src="https://github.com/FarzadMalik/4_class_activation_maps_visualization_algorithms/assets/107833662/3532684f-3854-4371-911e-2cc8b50d5cb2">


Let's dive into the notebook and uncover the exciting world of visualizing class activation maps using different algorithms. Happy learning and exploring!
