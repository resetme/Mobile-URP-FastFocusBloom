# Mobile-URP-FastFocusBloom
URP Bloom effect for mobile decvices

After profiling in many devices and sharing information with Unity Forum, we all realize that Unity new URP Post Effect is nor suitable for all mobile devices.

- Size of Build 
- Time of Build
- Increase Time of Shader Compile
- Decrease in almost 20 FPS in some devices
- GPU stall
- GPU GMEM Load increase from Standard PipeLine
- Around 24 Draw Calls
- FullScreen

For all those reason i created new URP Fast Focus Bloom

- NO GPU GMEM allocations
- NO GPU stall
- Only 4 Draw Call
- Dual Filtering Sampling
- Bloom only run on the fragment with the effect (NOT FULLSCREEN)
- - This Technique is used in many "AAA" mobile games.

## Profile

- Own Fast Focus Bloom is less than 1 MS on Snapdragon 820. (Increase with amount of objects)

![Image](https://github.com/resetme/Mobile-URP-FastFocusBloom/blob/main/GitFiles/OPT.png)


