# Video-Frame-Sync
Lines up frames between videos that are off slightly due to framerate, dropped/duplicated frames, etc.

Download link: https://github.com/pftq/Video-Frame-Sync/releases/tag/20261102<br>
You may also find these useful (one-click to download all [here](https://drive.google.com/drive/folders/1nvQFC5uwsZlf-82LuskCP-qut9xHw-lt?usp=sharing)):\
• [Video Debanding](https://github.com/pftq/Video-Debanding) (fixes quality issues with repeat re-processing/compression)\
• [Video Compare](https://github.com/pftq/Video-Compare) (to check export errors, differences, etc)\
• [MP4 Audio Delay Fix](https://github.com/pftq/MP4-Audio-Delay-Fix) (20ms delay at start of file)\
• [Video Color Match](https://github.com/pftq/VideoColorMatch) (correcting color grading drift)\
• [Video Splicer](https://github.com/pftq/Video-Splicer) (trim or join MP4s without re-encoding)\
• [Screencaps Generator](https://github.com/pftq/Screencaps-Generator) (smart screencaps selection + gallery grid sheet)

This is a tool I built for myself after having to deal with versions of the same footage often being slightly out of sync due to different framerates or dropped/duplicate frames.  This handles footage that is the same except for differences in specific spots (edits).  It'll line up the rest of the frames so they're in sync again, and for any dropped frames, it'll interpolate between the two existing neighboring frames.  This is also useful for AI video generation services that supposedly let you edit footage but often gives you back footage with dropped/duplicate frames as well (Seedance, etc).

An additional plus feature is it'll also match the color grading, contrast, slight sizing/position differences, etc.  It also supports references where the input video is shorter or a subset of the video you're trying to fix.

<img width="803" height="684" alt="image" src="https://github.com/user-attachments/assets/966529a9-af7a-41d4-908c-ad3dd86feea6" />

<img width="772" height="55" alt="image" src="https://github.com/user-attachments/assets/8a502651-0fef-4679-8a2a-f3a78b18c86f" />

Credits:
- [Python](https://www.python.org/) — application runtime
- [Tcl/Tk](https://www.tcl.tk/) via Tkinter — desktop interface
- [PyAV](https://github.com/PyAV-Org/PyAV) and
  [FFmpeg](https://ffmpeg.org/) — media decoding and encoding
- [OpenCV](https://opencv.org/) — image processing and optical flow
- [NumPy](https://numpy.org/) — numerical processing
- [Pillow](https://python-pillow.org/) — image previews
- [PyInstaller](https://pyinstaller.org/) — Windows application packaging
