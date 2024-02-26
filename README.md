# AWS EC2 Instance Management using Hand Gestures
![Running GIF](https://camo.githubusercontent.com/1140a4f2ffe1d7d5432df78421909e56c97909423568e609983ec3d4fbcb0b22/68747470733a2f2f726561646d652d747970696e672d7376672e6865726f6b756170702e636f6d3f666f6e743d4f72626974726f6e2673697a653d343026636f6c6f723d253233373941353030266865696768743d3637266475726174696f6e3d333030302663656e7465723d74727565266c696e65733d254630253946253835254236254630253946253836253831254630253946253835254234254630253946253835254234254630253946253836253833254630253946253835254238254630253946253835254244254630253946253835254236254630253946253836253832)


This code demonstrates how to manage AWS EC2 instances using hand gestures captured by a webcam. It uses the OpenCV library for capturing webcam video and the `HandTrackingModule` from the `cvzone` library to detect hand gestures. The code allows launching and terminating EC2 instances based on detected gestures.

## How the Code Works

The code does the following:

1. Captures webcam video using OpenCV.
2. Detects hand gestures using the `HandTrackingModule`.
3. Recognizes hand gestures to trigger AWS EC2 instance actions.
   - Index finger up: Launch an EC2 instance.
   - Thumb up: Terminate the most recently launched EC2 instance.
4. Manages AWS EC2 instances based on detected gestures.

## Usage

1. Make sure you have OpenCV and `cvzone` installed: `pip install opencv-python-headless cvzone boto3`.

2. Configure your AWS credentials using `aws configure` or by setting environment variables.

3. Replace the values in the `ImageId` and `SecurityGroupIds` parameters in the `myOSLaunch` function with your own values.

4. Run the script using a Python interpreter.

5. The script will open a webcam feed. Use hand gestures to launch and terminate AWS EC2 instances.

## Notes

- The code assumes that you have an active AWS account and appropriate permissions to manage EC2 instances.
- This code provides a basic example of using hand gestures to control AWS resources.

## Important

- Please exercise caution when using AWS resources and be aware of potential costs associated with running EC2 instances.
![Running GIF](  https://raw.githubusercontent.com/trinib/trinib/82213791fa9ff58d3ca768ddd6de2489ec23ffca/images/footer.svg)
