# Hamilton-Karaoke!

Welcome to The Hamilton Karaoke Project!

This project seeks to create a set of files to enable people to produce Karaoke videos using the Hamilton Original Broadway Cast Recording.

The HKP is based on [Karaoke Builder Studio](http://www.karaokebuilder.com/kbstudio.php), Windows-based software that can help construct karaoke tracks, build them into standard CDG files, and convert CDG and audio into .AVI files.  If you want to work with video files (either to contribute no-audio versions or to attach audio to a download) you'll want to install [VirtualDub](http://www.virtualdub.org/) as well.

The HKP does *not* contain any audio files (.mp3, .wav, etc) or files that contain audio (.bin, .avi).  (Any video files contributed MUST NOT have audio attached.)  Participants should acquire their own copy of the soundtrack.  If a disagreement arises about audio timing in a project file, the canonical reference timing is that of the MP3s available for download from Amazon (free with purchase of [the album](https://smile.amazon.com/Hamilton-Original-Broadway-Recording-Explicit/dp/B013JLBPGE)).

## Software Setup

* Karaoke editing
  * Download and install [Karaoke Builder Studio](http://www.karaokebuilder.com/kbstudio.php)
* Video creation
  * Download and install [VirtualDub](http://www.virtualdub.org/) for attaching sound to AVIs or for recompressing videos.
  * Install the [HuffYUV 2.11 Codec](https://www.videohelp.com/software/HuffYUV) for producing losslessly-encoded videos from Karaoke Builder Studio
  * Install [x264vfw Codex](https://sourceforge.net/projects/x264vfw/) for compressing videos into much smaller files.
* Audio-stripping (if chorus/etc is desired)
  * Download and install [Audacity](http://www.audacityteam.org/) for creating de-vocalized versions of songs


## Introduction to Karaoke Builder Studio

Karaoke Builder Studio is the software used to build .cdg files and convert them into .avi files.  The software allows users to create a .kbp 'project' that lays out the lyrics and set the timing of the 'wipe'.  KBS is free to download and use for creating/editing .kbp files, but requires registration (~$100) to enable .cdg and .avi creation.  **You can still contribute with the free version.**  You'll just need to rely on other contributors to convert your .kbp into .cdg or .avi files.

Here are some links to help you understand the software:


1. [Official website](http://www.karaokebuilder.com/kbstudio.php)
1. Watch jdcrooner's YouTube tutorial videos (particularly 1-3 and 6):
  1. Part 1: [Initial setup, lyrics, syllables, styles](https://www.youtube.com/watch?v=oHWG_HSflYM)
  1. Part 2.1: [Page layout, syllables](https://www.youtube.com/watch?v=NN9QfcHMgHs)
  1. Part 2.2: [Page layout, initial sync](https://www.youtube.com/watch?v=L65zSNwrAxM)
  1. Part 3.1: [Display tweaks, display/remove](https://www.youtube.com/watch?v=eSYdtKwVpRA)
  1. Part 3.2: [Lyric Sweeping (timing), display/remove](https://www.youtube.com/watch?v=wzeh80hzgMc)
  1. Part 4: [Creating a progress bar](https://www.youtube.com/watch?v=4IOMdRjDcg4)
  1. Part 5: [Slideshows](https://www.youtube.com/watch?v=4BLLZVdm6Xk)
  1. Part 6: [Finishing, splash screens](https://www.youtube.com/watch?v=4BLLZVdm6Xk)




## The Process

The process described below basically 

1. [Create or acquire the de-vocalized version of the song.](instructions/devocalizing.md)
1. [Choose colors for the parts](instructions/choose-colors.md)
1. [Lay out the lyrics](instructions/lay-out-lyrics.md)
1. [Sync the (dominant) lyrics to the music (w/ vocals) to produce a project file](instructions/initial-sync.md)
1. [Complete the first draft: assign styles and restore missing parts](instructions/complete-first-draft.md)
1. [Iteratively edit the lyric sweeping and line display times until satisfied](instructions/edit-display.md) (you will never be satisfied)
1. [Create the video(s)](instructions/create-videos.md)


