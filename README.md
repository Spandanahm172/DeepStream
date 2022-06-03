# DETECTING THE DIRECTION OF A VEHICLE
This application helps us in finding the direction in which the person is traversing. It is built on Nvidia Deepstream 5.1.
![Screenshot from 2022-06-03 15-37-05](https://user-images.githubusercontent.com/48898785/171841388-660b7255-4744-46d0-b032-3a70f881e11a.png)
# Deepstream Setup
This post assumes you have a fully functional Jetson device. If not, you can refer the documentation [here](https://docs.nvidia.com/jetson/jetpack/install-jetpack/index.html).
# 1. Install System Dependencies

        sudo apt install \
        libssl1.0.0 \
        libgstreamer1.0-0 \
        gstreamer1.0-tools \
        gstreamer1.0-plugins-good \
        gstreamer1.0-plugins-bad \
        gstreamer1.0-plugins-ugly \
        gstreamer1.0-libav \
        libgstrtspserver-1.0-0 \
        libjansson4=2.11-1
# 2.2. Install Deepstream
Download the DeepStream 5.1 Jetson Debian package deepstream-5.1_5.1.0-1_arm64.deb, to the Jetson device from here. Then enter the command:

        sudo apt install deepstream-5.1_5.1.0-1_arm64.deb
For more information, click here.
# 3. Clone the repository
        git clone https://github.com/anu-shreya/person_direction_deepstream.git
        cd person_direction_deepstream
# 4. Run the application
I. To build the application
        make
II. Now, run the application by providing the video source path
        ./person_direction_deepstream <h264_elementary_stream>
# Please find the Link of a Demo video below
[video](https://youtu.be/JuYdXGB2WiU)
