# Believengineers
Exploring the reliability of affordable AI-powered webcam-based pose estimation for measuring rehabilitation movements without expensive specialized equipment

RehabSense: Webcam-Based Rehabilitation Movement Monitoring

1. Project Purpose

RehabSense explores whether an ordinary laptop webcam combined with artificial intelligence (AI) can measure arm movement and detect compensatory trunk leaning during rehabilitation exercises. Following a stroke, some individuals may lean their trunk to compensate for arm weakness when raising their arms. Detecting these movements may help users and occupational therapists monitor movement quality and observe changes over time. The project evaluates whether an affordable webcam-based system could support preliminary rehabilitation monitoring.

2. How It Works

The system uses AI-powered pose estimation to identify body landmarks, including the shoulders, elbows, wrists and torso. Using the detected coordinates, Python calculates the right and left arm angles and trunk inclination angle. These measurements are displayed on screen, alongside a red “Trunk leaning detected!” alert when trunk inclination exceeds a predefined threshold of 5°. Users can optionally record their measurements after each session to track changes over time.

3. Technology Used

- Python: Calculates body angles and manages the system’s outputs
- MediaPipe: Detects body landmarks from webcam images
- OpenCV: Captures and processes video frames for movement analysis
- NumPy: Performs vector calculations to estimate arm elevation angles
Together, these tools enable real-time, webcam-based movement measurement without specialised motion-capture equipment.

4. Experiments and Results
   
The prototype was tested under different recording conditions to investigate its performance. These included increasing the distance between the user and webcam, reducing lighting levels, and changing laptop positioning. The system’s angle measurements were also compared with reference measurements to assess accuracy. Testing showed that the system could measure arm angles and detect potential trunk leaning at greater distances and under dimmer lighting, while stable laptop positioning was important for reducing inaccurate measurements.

5. Limitations

Despite working at further distances and in dimmer lighting, proper laptop alignment is required for reliable calculated measurements. The 5° trunk-leaning threshold is a predefined experimental setting rather than a clinically validated standard. Additionally, the prototype does not automatically store measurements or establish clinical recovery; users must record their results manually if they wish to compare progress over time. Therefore, RehabSense is an exploratory prototype and is not intended to replace professional rehabilitation assessment.
8. How to Run the Project
Step 1: Install Python and the required libraries listed in Requirements
Step 2: Run the program using the python code under rehab
Step 3: Allow access to your laptop webcam to observe real-time arm elevation and trunk inclination measurements
Step 4: Press Q to exit the program
