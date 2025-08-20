# Aircraft Recognition using Vision Transformer (ViT)

This project implements **aircraft recognition** using **Vision Transformers (ViTs)**, leveraging deep learning for fine-grained image classification. The system can accurately recognize over 100 different aircraft variants from the **FGVC Aircraft Dataset**.

Unlike conventional CNN-based methods, Vision Transformers process images as sequences of patches and utilize self-attention to capture both local and global dependencies. This results in improved accuracy and efficiency in classification tasks.

---

## Project Structure

* `index.html` – A sample webpage for interface demonstration
* `app.py` – Backend Flask application (for deployment/inference)
* `vit.py` – Vision Transformer model implementation and training script
* `sample_images/` – Sample aircraft images for testing
* `trained_aircraft_model/` – (Optional) Pre-trained model directory (if provided)

> **Note:** The full **FGVC Aircraft dataset** is not uploaded here due to size limitations. Please download it directly from:
> 👉 [FGVC Aircraft Dataset](https://www.robots.ox.ac.uk/~vgg/data/fgvc-aircraft/)

---

## Setup Instructions

### 1. Clone Repository

```bash
git clone https://github.com/your-username/aircraft-recognition-vit.git
cd aircraft-recognition-vit
```

### 2. Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate   # On Linux/Mac
venv\Scripts\activate      # On Windows
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

Main dependencies include:

* Python 3.8+
* PyTorch / TensorFlow
* Hugging Face Transformers
* Flask (for app.py)

### 4. Download Dataset

Download the **FGVC Aircraft Dataset** and place it in the project directory:

```
dataset/
 └── fgvc-aircraft-2013b/
      ├── images/
      ├── data/
```

### 5. Training (Optional)

If you want to train the model from scratch:

```bash
python vit.py
```

### 6. Running the App

After training or placing a pre-trained model inside `trained_aircraft_model/`, run:

```bash
python app.py
```

Then open your browser at `http://127.0.0.1:5000/` to test the web interface.

---

## Results

* Fine-grained classification of **100+ aircraft variants**
* Improved accuracy compared to CNN-based baselines
* Scalable and adaptable for real-world applications (aviation management, defense, inventory systems)

---

## References

This work is inspired by the FGVC Aircraft dataset and Vision Transformer (ViT) research:

* Dosovitskiy et al., *An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale* (NeurIPS 2020)
* FGVC Aircraft Dataset: [Official Website](https://www.robots.ox.ac.uk/~vgg/data/fgvc-aircraft/)

---

## Contact

For any questions, dataset setup, or guidance on running the model, please contact:
📧 **[ddhanus047@gmail.com](mailto:ddhanus047@gmail.com)**

