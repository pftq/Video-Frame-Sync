# Video-Frame-Sync
Lines up frames between videos that are off slightly due to framerate, dropped/duplicated frames, etc.

This is a tool I built for myself after having to deal with exports of the same footage sometimes having slightly different framerates or dropped/duplicate frames.  It'll line up the frames so they're in sync again and for any dropped frames, it'll interpolate between the two existing neighboring frames.  This is also useful for AI video generation services that supposedly let you edit footage but often gives you back footage with dropped/duplicate frames as well (Seedance, etc).
