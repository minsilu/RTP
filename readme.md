# Video Streaming Application

## 1. Environment Setup

Ensure your system has the following dependencies installed:

```
python == 3.6
pyqt5 == 5.10
opencv-python == 4.1.1.26
```


## 2. Launch Instructions

Follow the steps below to start the server and client. Make sure to execute the following commands from their respective `src` directories.

### Starting the Server

Example:

```
server: python Server.py serverPort 

client: python Client.py 127.0.0.1 serverPort rtpPort
```

```
python Server.py 1024

python Client.py 127.0.0.1 1024 1025
```

## Operating Instructions:

1. **Video Selection and Setup:**
   - Upon entering the interface, the right-hand side will automatically display all video files in the server's `src/video` directory.
   - Click on a video to select it and press the 'setup' button to load it. If no video is selected, the first video in the list will be loaded by default.

2. **Playback Controls:**
   - After setup, click the 'play' button to start the video. You can pause the video by clicking the 'pause' button.
   - Alternatively, toggle between play and pause using the spacebar, and adjust the video progress using the left and right arrow keys or by dragging the progress bar.

3. **Playback Speed:**
   - Use the three buttons at the bottom of the interface to switch between different playback speeds.

4. **Teardown and Video Switching:**
   - Click 'Teardown' to stop the current playback and revert to the initial unloaded state. You can then setup another video by repeating the setup process.
   - To switch videos, follow this flow: Teardown -> Select Video from Playlist -> Setup -> Play -> Teardown -> ...

5. **Video File Location:**
   - All videos to be played must be located in the server's `src/video` directory.

6. **Subtitle Files:**
   - Subtitle files for the client are automatically loaded based on the video name and should be placed in the same directory as `Client.py`.





