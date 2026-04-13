# Fine-tune-pre-trained-model
This project focuses on Image Classification by fine-tuning a pre-trained GoogLeNet model using PyTorch. The system is specifically trained on the Bean Leaf Lesions dataset from Kaggle to identify and categorize various diseases in bean plants through transfer learning.
🌱 Bean Leaf Lesion Classification (Fine-Tuning)
This repository demonstrates how to perform transfer learning on a deep convolutional neural network. By leveraging a pre-trained GoogLeNet architecture, the model is adapted to classify specific agricultural diseases with high accuracy and reduced training time.

🚀 Features
Transfer Learning: Fine-tunes a pre-trained GoogLeNet model by modifying the final fully connected layer to match the number of target classes.

Automated Dataset Access: Integrated with the opendatasets library for seamless downloading of the Bean Leaf Lesions dataset from Kaggle.

Advanced Training Loop: Implements a robust training process with CrossEntropyLoss and the Adam Optimizer.

Performance Tracking: Monitors and plots both training loss and accuracy across epochs to visualize model convergence.

🛠️ Tech Stack
Framework: PyTorch

Model Architecture: GoogLeNet (Inception v1)

Data Handling: NumPy, Pandas, Scikit-learn (LabelEncoder)

Vision Tools: Torchvision (Transforms and ImageFolder)

Environment: Google Colab / Jupyter Notebook

📂 Dataset
The model is trained on the Bean Leaf Lesions Classification dataset, which includes images categorized into:

Angular Leaf Spot

Bean Rust

Healthy

🔧 Setup & Usage
Clone the Repository:

Bash
git clone https://github.com/yourusername/bean-lesion-classification.git
Kaggle Setup: Ensure your kaggle.json is available to facilitate the automated dataset download.

Execution: Open Fine_tune_pre_trained_model(image_classification).ipynb and run the cells. The notebook will handle data extraction, model modification, and training.

Inference:
The model evaluates validation data using torch.no_grad() to ensure efficient performance testing without updating weights.

🧠 Technical Workflow
Preprocessing: Images are resized, normalized, and converted to tensors.

Model Adaptation: The pre-trained weights of GoogLeNet are loaded, and the output layer is replaced to output 3 classes.

Optimization: The model uses a learning rate-optimized Adam optimizer to fine-tune the weights for the new dataset.
