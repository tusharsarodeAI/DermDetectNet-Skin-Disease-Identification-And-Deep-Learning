
# 🩺 **DermDetectNet: Skin Disease Identification Using ResNet-50 and Flask**

**DermDetectNet** is an AI-powered web application that uses the **ResNet-50** deep learning model to identify and classify skin diseases from uploaded images. The model not only predicts the **disease name** but also provides **detailed information** about the detected disease to assist users in understanding the condition.

---

## 🚀 **Features**

✅ **Image Upload:** Users can upload skin lesion images for disease identification.  
✅ **Disease Classification:** Uses ResNet-50 to identify multiple skin diseases.  
✅ **Disease Information:** Provides detailed information, symptoms, and treatment for detected diseases.  
✅ **Confidence Score:** Displays the confidence level of the prediction.  
✅ **User Dashboard:** View and manage past diagnoses.  
✅ **Real-Time Prediction:** Quick and accurate results using pre-trained deep learning models.  

---

## 🛠️ **Tech Stack**

| Technology         | Description                           |
|--------------------|---------------------------------------|
| **Python**          | Backend API using Flask               |
| **Flask**           | Lightweight web framework             |
| **ResNet-50**       | Pre-trained CNN model for classification |
| **TensorFlow/Keras**| Deep learning framework               |
| **HTML/CSS**        | Frontend styling                      |
| **AWS/GCP**         | Cloud platform for hosting            |

---

## 📚 **Dataset**

- **ISIC (International Skin Imaging Collaboration) Dataset**
- Includes thousands of labeled skin lesion images used to fine-tune the **ResNet-50** model for multi-class classification.

---


## ⚡️ **Model Prediction Workflow**

1. **Image Upload:** User uploads a skin lesion image.  
2. **Preprocessing:** Image is resized and normalized.  
3. **Model Prediction:** ResNet-50 model classifies the image.  
4. **Disease Name & Information:** Retrieves disease information from `disease_data.json`.  
5. **Result Display:** Shows disease name, confidence score, and detailed information.  

---

## 📚 **Disease Information (disease_data.json)**

```json
{
  "Melanoma": {
    "description": "Melanoma is a type of skin cancer that develops from the pigment-producing cells known as melanocytes.",
    "symptoms": [
      "Asymmetrical moles",
      "Irregular borders",
      "Varied color",
      "Increase in size"
    ],
    "treatment": "Treatment includes surgical removal, chemotherapy, and radiation therapy."
  },
  "Benign Nevus": {
    "description": "Benign nevi are non-cancerous moles that often appear on the skin.",
    "symptoms": [
      "Evenly colored mole",
      "Symmetrical shape",
      "Does not change over time"
    ],
    "treatment": "No treatment is required unless there are cosmetic concerns."
  },
  "Seborrheic Keratosis": {
    "description": "Seborrheic keratosis is a common, non-cancerous skin growth that appears as a waxy, brown, or black lesion.",
    "symptoms": [
      "Rough or scaly texture",
      "Waxy appearance",
      "No pain or itching"
    ],
    "treatment": "Treatment includes cryotherapy, curettage, or laser therapy."
  }
}
```

---

## 🚦 **API Endpoints**

| Endpoint              | Method | Description                   |
|-----------------------|--------|-------------------------------|
| `/api/predict`         | POST   | Upload and predict disease    |
| `/api/user/register`   | POST   | Register new user             |
| `/api/user/login`      | POST   | User login                    |
| `/api/history`         | GET    | Retrieve prediction history   |



## 📊 **Evaluation Metrics**

- **Accuracy:** 89.5%  
- **Precision:** 86%  
- **Recall:** 86.5%  
- **F1 Score:** 88%  

---

## 📝 **Future Enhancements**

✅ Expand model to identify more skin diseases.  
✅ Add multi-language support.  
✅ Integrate chatbot for user consultation.  
✅ Create a mobile app using **React Native**.  

---

## 🤝 **Contributing**

Contributions are welcome! To contribute:
- Fork the repository.
- Create a new branch.
- Make your changes and commit.
- Submit a pull request.

---

## 📧 **Contact**

- **Author:** Tushar Sarode  
- **Email:** [tusharsarode0228@gmail.com](mailto:tusharsarode0228@gmail.com)  

---

## 🎉 **Acknowledgements**

Special thanks to:
- **ISIC Dataset Contributors**  
- Open-source community for continuous learning and support.  

---

💡 **Star the repo if you find this helpful!** ⭐️  
Happy Coding! 🎯
