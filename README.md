# gst-tutorial5-rtsp
GStreamer tutorial 5 project working with GStreamer SDK 1.6.0 

Currently this project has been tested and builds in Eclipse Mars.1 on Windows 8.1

Just set Environment Variables GSTREAMER_SDK_ROOT and GSTREAMER_SDK_ROOT_ANDROID to the location of your GStreamer for Android 1.6.0 directory

Also, when the project is open go to its Properties->Builders, and ensure there is a Program builder called 'NDK_tutorial5' there, as this is what allows it to build properly. I was unable to get Android->Add Native Support... to work so this builder is used instead.

Currently not working: RTSP streaming of H264 encoded video doesn't work, and that is the end goal of this project. It appears that a UDP connection is established but no data is transferred so it times out and gives up.
