<p align="center">
  <img src="https://imgur.com/kcpxcCv.png" alt="Architecture Diagram" width="600"/>
</p>

## ☁️ Building an Image Labels Generator using Amazon Rekognition

This project demonstrates how to build an image label detection tool using **Amazon Rekognition**. With this tool, you can upload an image to an S3 bucket, and Amazon Rekognition will identify and label individual parts of the image (e.g., objects, scenes) with confidence scores.

---

## 🧰 Technologies Used

- Python
- boto3 (AWS SDK for Python)
- Amazon Rekognition
- Amazon S3
- AWS CLI
- IAM (for access control)

---

## 🛠️ How It Works

1. **Upload an image to S3**
   - Create a bucket and upload the image you'd like to analyze.

2. **Configure AWS CLI**
   - Run `aws configure` and provide:
     - Access key
     - Secret key
     - Region (should match the region of your S3 bucket)

3. **Install Required Python Libraries**
   ```bash
   pip install boto3 matplotlib pillow

## 🧑‍💻 Write and Run Your Python Code

### 1. Implement the Script

Use the following libraries and functions to build your image label detection tool:

- **`boto3`**  
  - Connect to your S3 bucket  
  - Call Amazon Rekognition’s `detect_labels()` method

- **`PIL (Pillow)`**  
  - Load the image retrieved from S3

- **`matplotlib`**  
  - Display the image  
  - Optionally draw bounding boxes around detected labels

---

### 2. Prepare Your Parameters

Before running the script:

- Upload the image you want to analyze to your S3 bucket
- Update the `photo` and `bucket` variables in your `rekognition.py` script with the actual file and bucket names

---

### 3. Run the Script

Use the following command to execute your program:

```bash
python rekognition.py
