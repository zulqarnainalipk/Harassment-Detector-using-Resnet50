<!-- Header Section -->
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: center; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <h1 style="color: #8e44ad; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); font-weight: bold; margin-bottom: 10px; font-size: 36px;">Harassment Detection Model</h1>
</div>

<hr style="border: 0; height: 1px; background: #ccc; margin-top: 20px; margin-bottom: 20px;">

<!-- Project Overview Section -->
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: center; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <h2 style="color: #8e44ad; font-size: 28px; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); margin-bottom: 15px;">Project Overview</h2>
</div>
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: left; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <p style="color: #3b3b3b; font-size: 18px;">
        In this project, we develop a <b>deep learning-based model</b> aimed at <b>detecting harassment</b> in images. The model classifies images into the following categories:
    </p>
    <ul style="color: #3b3b3b; font-size: 18px; text-align: left; margin-left: 20px;">
        <li><b>Victim</b>: The individual who is being harassed.</li>
        <li><b>Perpetrator</b>: The individual engaging in the harassing behavior.</li>
        <li><b>Unwanted Touching</b>: Instances of physical contact without consent.</li>
    </ul>
</div>
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: left; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <p style="color: #3b3b3b; font-size: 18px;">
        This project leverages <b>object detection</b> and <b>classification</b> techniques to identify instances of harassment from images, contributing towards <b>real-time monitoring</b> and <b>prevention</b> of harassment in various environments.
    </p>
</div>

<hr style="border: 0; height: 1px; background: #ccc; margin-top: 20px; margin-bottom: 20px;">

<!-- Problem Statement Section -->
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: center; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <h2 style="color: #8e44ad; font-size: 28px; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); margin-bottom: 15px;">Problem Statement</h2>
</div>
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: left; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <p style="color: #3b3b3b; font-size: 18px;">
        Harassment is a prevalent and harmful issue, especially in public spaces like transportation, workplaces, and social settings. Despite its gravity, incidents of harassment often go unnoticed or unreported. This project aims to <b>automate the detection of harassment</b> from images, offering potential solutions for <b>real-time identification</b>, improving safety, and enhancing public awareness.
    </p>
</div>
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: left; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <p style="color: #3b3b3b; font-size: 18px;">
        By creating an automated system that classifies images into <b>Victim</b>, <b>Perpetrator</b>, and <b>Unwanted Touching</b>, the goal is to help <b>identify harassment</b> in a timely manner and create <b>safer environments</b>. Through this, the project can assist authorities, organizations, or monitoring systems to take <b>swift action</b>.
    </p>
</div>

<hr style="border: 0; height: 1px; background: #ccc; margin-top: 20px; margin-bottom: 20px;">

<!-- Approach Section -->
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: center; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <h2 style="color: #8e44ad; font-size: 28px; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); margin-bottom: 15px;">Approach</h2>
</div>

<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: left; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <h3 style="color: #8e44ad; font-size: 24px; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); margin-bottom: 10px;">1. Data Collection and Annotation</h3>
    <p style="color: #3b3b3b; font-size: 18px;">
        The dataset consists of images with annotations in <b>XML</b> format. Each image is annotated with bounding box coordinates and class labels representing:
    </p>
    <ul style="color: #3b3b3b; font-size: 18px; text-align: left; margin-left: 20px;">
        <li><b>Victim</b></li>
        <li><b>Perpetrator</b></li>
        <li><b>Unwanted Touching</b></li>
    </ul>
</div>

<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: left; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <h3 style="color: #8e44ad; font-size: 24px; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); margin-bottom: 10px;">2. Preprocessing & Data Augmentation</h3>
    <p style="color: #3b3b3b; font-size: 18px;">
        Various <b>image preprocessing techniques</b> were applied, such as resizing the images to 224x224 pixels, and augmenting the dataset using horizontal flips, rotations, and color jitter to improve the model's generalization.
    </p>
</div>

<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: left; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <h3 style="color: #8e44ad; font-size: 24px; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); margin-bottom: 10px;">3. Model Architecture</h3>
    <p style="color: #3b3b3b; font-size: 18px;">
        The architecture used is <b>ResNet-50</b>, a powerful deep learning model known for image classification tasks. The model consists of:
    </p>
    <ul style="color: #3b3b3b; font-size: 18px; text-align: left; margin-left: 20px;">
        <li><b>ResNet-50 Backbone</b>: Pre-trained on ImageNet.</li>
        <li><b>Custom Fully Connected Layers</b>: Fine-tuned for our 3-class classification problem.</li>
    </ul>
</div>

<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: left; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <h3 style="color: #8e44ad; font-size: 24px; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); margin-bottom: 10px;">4. Training and Evaluation</h3>
    <p style="color: #3b3b3b; font-size: 18px;">
        We used <b>Cross-Entropy Loss</b> for training and <b>Adam Optimizer</b> for optimization. The performance of the model was evaluated using metrics like <b>accuracy</b>, <b>precision</b>, <b>recall</b>, and the <b>confusion matrix</b>.
    </p>
</div>

<hr style="border: 0; height: 1px; background: #ccc; margin-top: 20px; margin-bottom: 20px;">

<!-- Project Structure Section -->
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: center; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <h2 style="color: #8e44ad; font-size: 28px; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); margin-bottom: 15px;">Project Structure</h2>
</div>

<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: left; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <pre style="background-color: #f1f1f1; color: #3b3b3b; font-family: 'Courier New', Courier, monospace; padding: 15px; border-radius: 10px;">
    ├── README.md                   # Project description and instructions
    ├── harassment_detection_model.pth  # Saved trained model
    ├── dataset/                     # Directory containing images and annotations
    │   ├── JPEGImages/              # Image files in .png format
    │   └── Annotations/             # XML annotation files
    ├── notebook.ipynb               # Jupyter notebook with full workflow
    ├── utils/                       # Utility functions for preprocessing
    │   └── data_utils.py
    └── requirements.txt             # Python package dependencies
    </pre>
</div>

<hr style="border: 0; height: 1px; background: #ccc; margin-top: 20px; margin-bottom: 20px;">

<!-- Instructions Section -->
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: center; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <h2 style="color: #8e44ad; font-size: 28px; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); margin-bottom: 15px;">Instructions</h2>
</div>

<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: left; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <p style="color: #3b3b3b; font-size: 18px;">
        1. Clone the repository: <code>git clone <i>repo_link</i></code><br>
        2. Install dependencies: <code>pip install -r requirements.txt</code><br>
        3. Run the Jupyter notebook to train and evaluate the model.<br>
        4. Optionally, you can use the pre-trained model for testing the harassment detection functionality.<br>
    </p>
</div>

<hr style="border: 0; height: 1px; background: #ccc; margin-top: 20px; margin-bottom: 20px;">

<!-- Conclusion Section -->
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: center; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <h2 style="color: #8e44ad; font-size: 28px; text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.2); margin-bottom: 15px;">Conclusion</h2>
</div>
<div style="border-radius: 15px; border: 2px solid #d5a6e5; padding: 20px; background-color: #e1f5f3; text-align: left; box-shadow: 0px 4px 8px rgba(0, 0, 0, 0.2);">
    <p style="color: #3b3b3b; font-size: 18px;">
        The development of this harassment detection model has the potential to make a positive impact in identifying harassment in real-world environments. By leveraging deep learning and computer vision techniques, the project contributes to the <b>fight against harassment</b> and <b>advocates for safer spaces</b>.
    </p>
</div>

Connect with me on Linkdin : https://www.linkedin.com/in/zulqarnainalipk/
