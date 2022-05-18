# Tensorflow Object Detection Walkthrough with Raspberry Pi

<b>Step 1.</b> Clone the current repository onto your Raspberry Pi or copy it from a machine using RDP.
<pre> git clone https://github.com/AditiRokade/detection </pre>
<br/><br/>
<b>Step 2.</b>Install the required dependencies onto your Raspberry Pi
<pre>
pip3 install opencv-python 
sudo apt-get install libcblas-dev
sudo apt-get install libhdf5-dev
sudo apt-get install libhdf5-serial-dev
sudo apt-get install libatlas-base-dev
sudo apt-get install libjasper-dev 
sudo apt-get install libqtgui4 
sudo apt-get install libqt4-testv
echo "deb https://packages.cloud.google.com/apt coral-edgetpu-stable main" | sudo tee /etc/apt/sources.list.d/coral-edgetpu.list
curl https://packages.cloud.google.com/apt/doc/apt-key.gpg | sudo apt-key add -
sudo apt-get update
sudo apt-get install python3-tflite-runtime
</pre>
<br/><br/>
<b>Step 3.</b> Copy your detect.tflite model into the same repository and update the labels.txt file to represent your labels. 
<br/><br/>
<b>Step 4.</b> Run real time detections using the detect.py script
<pre>python3 detect.py</pre>
<br/><br/>
