# smart-face-attendance
## Face Enrollment (enroll.py)

This script is used to add a new person to the face recognition system.
It opens the webcam, captures face images, and saves them so the system
can recognize the person later.

---

### What this script does
- Opens the webcam
- Detects faces in real time
- Saves multiple face images for one person
- Stores person details in a small database
- Shows progress using a simple GUI

---

### Dataset folder created
After enrollment, face images are saved in this format:

dataset/
└── PROJECT/
    └── PERSON_ID/
        ├── 00000.png
        ├── 00001.png
        ├── ...
        └── 000NN.png

---

### Database
- Uses TinyDB (JSON file based)
- Stores person ID, name, and enrollment status
- Prevents enrolling the same person twice

---

### Requirements
Before running the script, install the required libraries:

```bash
pip install -r requirements.txt
