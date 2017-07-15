# Creating Videos

We're almost finished!  Now we just need to produce the (music-free) AVIs so that others can use the video.


## Software
These steps require some additional software beyond Karaoke Builder Studio.


**[VirtualDub](http://www.virtualdub.org)** - This software allows you to recompress video and to change the audio track (or its timing) in a video.

**[HuffYUV 2.11 Codec](https://www.videohelp.com/software/HuffYUV)** - This is a lossless video codec that allows fast output from KBS that's slightly smaller than uncompressed video.

**[x264vfw Codex](https://sourceforge.net/projects/x264vfw/)** - This is a video codec for producing compressed video that takes up much less space (but takes longer to generate).


## Creating a video from KBS

This requires the full suite of software described above.

1. Build the CDG file outputs/output.cdg.
  1. Click 'Build' in Karaoke Builder Studio, select 'Build .CDG File'
  1. Specify 'outputs/output.cdg' in the song directory
  1. Click 'Save'
1. Convert the CDG file into an AVI (outputs/huffyuv-vocals.avi) in HuffYUV format with original vocal track
  1. Click 'Tools' 
  1. Inputs:
    1. Specify the aforementioned 'output.cdg' for 'CD+G'
    1. Specify the audio with the vocals for 'Audio'
  1. Specify 'outputs/huffyuv-vocals.avi'
  1. Select 'Huffyuv v2.1.1' as your Video Compressor
  1. Click 'Build', select 'Huffyuv v2.1.1', click 'OK'
1. Verify the output mostly works
  1. Open the video from Explorer and see that it works
  1. It might complain about 'This AVI was not prepared for sequential reading' - don't worry about that for now
  1. The timing might be slightly off as well - again don't worry about that.
1. Re-sync and recompress the video
  1. Open 'huffyuv-vocals.avi' in VirtualDub
  1. Click 'Play', see how well the timing matches up. Make sure 'Audio', 'Direct Stream Copy' is selected.
  1. Adjust the audio-track delay via 'Audio', 'Interleaving' menu. You may need to move it earlier (negative number) or later (positive number). ~250-275ms is not uncommon.
  1. Set up the video compression options
    1. Select 'Video', 'Full Processing Mode'
    1. Select 'Video', 'Compression...'
    1. Select 'x264vfw' code, click 'Configure'
    1. Make sure 'Zero Latency' is checked up top, and Output has 'VFW', 'H264' and 'VirtualDub Hack' all selected.  Click 'OK'.
  1. 'File', 'Save As AVI...'; save file as 'outputs/h264-vocals.avi'
1. Verify the output is good: timing is fine, visuals are fine
1. Create a no-audio version for uploading
  1. Open 'outputs/h264-vocals.avi' in VirtualDub
  1. Select 'Audio', 'No Audio'
  1. Select 'Video', 'Direct Stream Copy'
  1. 'File', 'Save As Avi...'; save file as 'outputs/h264-noaudio.avi'
1. Upload 'output.cdg' and 'h264-noaudio.avi' to GitHub and send a Pull Request.


## Attaching Audio to an existing video

If you're looking to change the audio attached to a video (e.g. you downloaded the audio-free video from GitHub) then follow these instructions.  The only software you need for this is VirtualDub (above).

1. Open the file in VirtualDub
1. 'Audio', 'Audio from other file...'; select the desired file
1. Select 'Video', 'Direct Stream Copy'
1. Click 'Play', see how well the timing matches up.
1. Adjust the audio-track delay via 'Audio', 'Interleaving' menu. You may need to move it earlier (negative number) or later (positive number). ~250-275ms is not uncommon.
1. 'File', 'Save As AVI...'; save file as whatever you want
