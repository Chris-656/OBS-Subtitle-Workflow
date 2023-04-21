# WORKFLOW

## SOFTWARE
The following software is used for the workflow.

-
- [OBS Studio](https://obsproject.com/de/download)
- [OBS Closed Captioning Plugin](https://github.com/ratwithacompiler/OBS-captions-plugin/releases), when transcribe is used LIVE within OBS. Postprocess use Subtitle Edit
- DaVinci Resolve
- [reCode](https://www.xmedia-recode.de/) to convert mp4 to mkv, to hold multiple subtitles
- [Subtitle Edit](https://www.nikse.dk/), Transscribe Option using whisper from video here available
- [App Key*n Strokes](https://github.com/Phaiax/Key-n-Stroke) for Highlight Cursor and Keystrokes. In OBS only screen capture is working no window capture.

## Workflow
  1. Record the video with OBS
     - Set Outputformat to mp4 or remux the mkv to mp4, otherwise frame drops can appear when using with davici resolve
  2. Cut the raw video in Premiere or daVinci Resolve
  3. Start subtitle edit
     - load video and generate subtitles with whisper
     - translate the subtitles into the appropriate language(s)
     - Add multiple subtitles to video (generate video with added subtitles)
     - export subtitles in vtt format to be used in MS Stream as seperate subtitles
