# Athlete Recognition System - Video-Based Player Identification (BYM 308 Final Project)

> A CNN-based AI system that automatically identifies specific athletes from video footage using deep learning.

## 📝 Project Overview
This project develops an automated solution for identifying athletes in videos using Convolutional Neural Networks (CNN). Designed for sports analytics, player tracking, and personalized statistics generation, the system processes user-uploaded videos to detect which athlete appears in the footage.

## 🛠️ Technical Implementation
### Approach
- **Data Preparation**: 30 images per athlete (22 athletes total)
- **CNN Architecture**: 
  - Layers: `Conv2D`, `MaxPooling2D`, `Flatten`, `Dense`
  - Input: 150x150px images (upgraded to 224x224 in improvements)
  - Classification: Multi-class via `Softmax`
- **Video Processing**: Frame-by-frame analysis with OpenCV

### Key Improvements
- Data augmentation (rotation, zoom, shifting)
- Early Stopping to prevent overfitting
- Increased model complexity with Dropout layers
- Higher resolution image processing (224x224)

## 📊 Results
Tested on 7 athletes including:
- Simone Biles
- Stephen Curry
- Cristiano Ronaldo
- Usain Bolt  
- Victor Osimhen  
- Naim Süleymanoğlu  
- Zinedine Zidane

**Notable Findings**: 
- Higher error rates for darker-skinned athletes
- Accuracy variations due to data imbalance and lighting differences
- Visual results output as bar charts with confidence percentages

## ⚙️ Tech Stack
`TensorFlow/Keras` | `OpenCV` | `Google Colab` | `Matplotlib` | `Python`

## 📁 Repository Structure
/
├── Data/ # Athlete image folders
├── Models/ # Trained CNN models
├── Video_Processing/ # Frame extraction & prediction scripts
├── Results/ # Output visualizations
├── Documentation/ # Project report & references
└── Main.ipynb # Colab implementation



## 👥 Team Contributions
| Member               | Role                                  |
|----------------------|---------------------------------------|
| Uğur Baki Arslan     | Model architecture & training         |
| Selami Çetin         | Video processing & visualization     |
| Yunus Emre Sevinç    | Testing, reporting & interpretation  |

## 🔍 Future Work
- Expand dataset with balanced athlete representation
- Improve lighting/color normalization
- Implement face recognition supplements
- Test with real-time video streams

- Key features of this description:

Includes all technical specifications from your slides

Highlights both achievements and observed limitations (bias issues)

Clearly defines team roles and responsibilities

Uses GitHub-friendly structure with emoji visual cues

Mentions future improvements potential

Maintains academic integrity with proper attribution

For best results on GitHub:

Create matching folders in your repo

Add screenshots of your result graphs in /Results

Include your Colab notebook as Main.ipynb

Add requirements.txt with package versions

Use relevant topics: #cnn #athlete-recognition #tensorflow #opencv #sports-analytics
