# Plant-Health-and-Disease-Detection
Plant Disease Recognition System using Custom CNN and MobileNetV2 on the PlantVillage dataset.

# Model Setup Instructions
To use this project, you need to download a pre-trained model from the given Google Drive link and place it in the `models` directory.

## Steps to Download and Place the Model

1. **Download the Model**
   - Click [here](https://drive.google.com/file/d/1Ond7UzrNOfdAXWedjlZr2sDXYU6MRBuj/view?usp=sharing) to open the Google Drive link.
   - Click the **Download** button to save the file to your local system.

2. **Create the Models Folder**
   - Navigate to the root directory of this project.
   - Create a folder named `models` if it does not already exist.
```bash
     mkdir models
```

3. **Place the Model in the Folder**
   - Move the downloaded file into the `models` directory.
```bash
     mv /path/to/downloaded/model models/
```

4. **Verify the Setup**
```bash
   ls models
```

## Usage

1. **Specify the Model File Location**
   - Open the `app.py` file in a text editor.
   - Locate line 8 and update it with the model path:
```python
     tf.keras.models.load_model("models/your_model_file.keras")
```
     Replace `your_model_file.keras` with the actual name of the downloaded file.

2. **Run the Server**
```bash
   python app.py
```

3. **Access the Application**
   - Once the server is running, open your browser and go to the URL shown in the terminal (usually `http://127.0.0.1:5000`).
