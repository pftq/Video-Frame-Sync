# Video-Frame-Sync
Lines up frames between videos that are off slightly due to framerate, dropped/duplicated frames, etc.

This is a tool I built for myself after having to deal with versions of the same footage often having slightly frame timings due to different framerates or dropped/duplicate frames.  This handles footage that is the same except for differences in specific spots (edits).  It'll line up the rest of the frames so they're in sync again and for any dropped frames, it'll interpolate between the two existing neighboring frames.  This is also useful for AI video generation services that supposedly let you edit footage but often gives you back footage with dropped/duplicate frames as well (Seedance, etc).

<img width="803" height="684" alt="image" src="https://github.com/user-attachments/assets/966529a9-af7a-41d4-908c-ad3dd86feea6" />
