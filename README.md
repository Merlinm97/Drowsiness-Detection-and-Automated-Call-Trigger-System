Drowsiness Detection and Call Trigger using Facial Landmarks

This project implements a drowsiness detection system that processes a video file to detect facial features and triggers a call using Twilio when drowsiness is detected.

Key Features:

Load Models: Loads dlib's face detector and shape predictor for extracting facial landmarks.
Video Input: Processes a video file frame by frame.
Face Detection: Detects faces in each frame and extracts facial landmarks.
EAR and MAR Calculation: Calculates the Eye Aspect Ratio (EAR) and Mouth Aspect Ratio (MAR) to assess eye and mouth states.
Drowsiness Detection: Tracks drowsiness based on eye and mouth states (eyes closed or mouth open). If drowsiness is detected for more than the specified time (DROWSY_TIME_THRESHOLD), it triggers a call to a specified phone number using the Twilio API.
Bounding Box and Display: Draws a bounding box around the face and displays the status of the eyes, mouth, and overall drowsiness state on the frame.
Trigger Call: If drowsiness lasts for the set duration, a call is triggered using the Twilio API.

Notes:
Replace account_sid, auth_token, and phone_number with your actual Twilio credentials and phone number.
The video is processed frame-by-frame, and when drowsiness is detected for the specified duration, a call is triggered.

