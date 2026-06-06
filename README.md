# FaceScope: Zodiac-Sign-Prediction-from-Facial-Features
An experimental Python computer vision project that analyzes facial similarity among celebrities and attempts to predict a person's zodiac sign based solely on facial features. The model is trained on celebrity face datasets grouped by birth sign and uses image similarity techniques to find visual patterns associated with each zodiac category.

## FaceScope is an experimental machine learning and computer vision project that explores a popular internet claim: *do people born under the same zodiac sign tend to look alike?*

Using a dataset of celebrity faces labeled by zodiac sign, the project:

Collects celebrity images and birth dates
Automatically assigns zodiac signs from birthdays
Detects and crops faces
Extracts facial representations using OpenCV
Compares facial similarity across zodiac groups
Predicts which zodiac sign a new face most closely resembles

Rather than attempting to validate astrology, FaceScope investigates whether a facial similarity model can identify visual patterns within groups of people who share the same zodiac sign.

- How It Works
  - Dataset Creation
  - Celebrity names, birthdays, and image URLs are collected.
  - Birthdays are converted into zodiac signs.
- Image Processing
  - Images are downloaded automatically.
  - Faces are detected using OpenCV Haar Cascades.
  - Facial regions are cropped and standardized.
- Training
  - Faces are organized into 12 zodiac categories.
  - Each face is converted into a numerical representation.
  - Encodings are stored by zodiac sign.
- Prediction
  - A new face is uploaded.
  - The model compares it against all training faces.
  - The most similar faces vote on the predicted zodiac sign.
  - Confidence scores and similarity metrics are returned.

*Can a computer guess your zodiac sign from your face? Probably not accurately, but it's fun to find out.*
