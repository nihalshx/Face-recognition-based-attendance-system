
# 🎓 Face Recognition-based Attendance System

This project is a **Face Recognition-based Attendance System** that automates attendance recording using a webcam and a machine learning model. It includes a Flask-based web application to manage users and attendance records.

---

## ✨ Features

- 📸 **Face Detection**: Detect faces using OpenCV's Haar cascades.
- 🧑‍🤝‍🧑 **Face Recognition**: Identify users with a KNN-based classifier.
- 🕒 **Attendance Recording**: Automatically logs attendance with the user's name, ID, and timestamp.
- ➕ **Add New Users**: Capture and register new faces for recognition.
- 📂 **Daily Attendance Logs**: Stores attendance in daily CSV files.
- 🌐 **Web Interface**: Simple UI to manage attendance and users.

---

## 🛠️ Prerequisites

1. **Python 3.7 or higher**
2. **Required Python libraries**:
   - `Flask`
   - `OpenCV`
   - `scikit-learn`
   - `joblib`
   - `numpy`
   - `pandas`

   Install dependencies using:
   ```bash
   pip install -r requirements.txt
   ```

3. **Haar Cascade file**:
   - Download `haarcascade_frontalface_default.xml` and ensure it is in the project directory.

---

## 📁 Directory Structure

```
Attendance/
  - Attendance-{MM_DD_YY}.csv   # Daily attendance logs
static/
  - face_recognition_model.pkl  # Trained ML model
  - faces/                      # Registered user faces
templates/
  - home.html                   # Web interface template
app.py                          # Main application script
```

---

## 🚀 How to Run

1. **Clone this repository**:
   ```bash
   git clone <repository-url>
   cd face-recognition-attendance
   ```

2. **Run the Flask app**:
   ```bash
   python app.py
   ```

3. **Open the web app in your browser**:
   ```
   http://127.0.0.1:5000/
   ```

---

## 📖 Usage

### ➕ Add New Users
1. Navigate to the "Add User" page.
2. Enter a unique name and ID for the user.
3. Capture images using the webcam.
4. The system will train the recognition model automatically.

### 🕒 Record Attendance
1. Click on the "Take Attendance" button.
2. The webcam will start and recognize registered faces.
3. Attendance will be logged in the CSV file.

---

## 📝 Notes

- Ensure proper lighting for better face detection.
- The system uses a **K-Nearest Neighbors (KNN)** classifier for recognition.
- Daily attendance is saved in `Attendance/Attendance-{MM_DD_YY}.csv`.

---

## 🌟 Future Enhancements

- 🔍 Enhance face recognition with deep learning (e.g., using a pre-trained model like FaceNet).
- 🛠️ Add user management features (e.g., edit or delete users).
- 📊 Export attendance logs in other formats (e.g., Excel, PDF).
- ☁️ Integrate with cloud storage for centralized attendance records.

---

Feel free to contribute, fork, and ⭐ the repository if you find it useful!

