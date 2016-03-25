Consolodated Vision Advice
==========================

1) RGB filtering might be faster than HSL

2) Doing Kalman filtering on targets will probably help reduce jitter

3) For rotating to face a target: a gyroscope will be nessessary. An
ardupilot doesn't cut it.

4) GRIP is nice for setting up a pipeline, but 78 reccomends using
OpenCV for actual vision.

5) Remember to account for backlighting

6) Auto white balance might be hurting you

7) Fighting to get GRIP deployed probably isn't worth your time. See #4
