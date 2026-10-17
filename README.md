# Plugg Lab (VST3 instrument for FL Studio)

Voices: Soft Bell, Glass Pluck, Tropical Pad, Bright Lead.
Knobs: Attack, Release, Bright, Tone (centre = as designed), Chorus, Reverb, Level.
Re-skin: edit colours in Source/Theme.h.

## Build (needs CMake 3.22+ and internet on first configure, JUCE downloads itself)

Windows: install Visual Studio 2022 with "Desktop development with C++" and CMake.
Mac: install Xcode command line tools and CMake.

    cmake -B build
    cmake --build build --config Release

Result: build/PluggLab_artefacts/Release/VST3/Plugg Lab.vst3
Copy that folder to:
  Windows: C:\Program Files\Common Files\VST3
  Mac:     /Library/Audio/Plug-Ins/VST3
Then in FL Studio: Options > Manage plugins > Find installed plugins.

## No compiler? Build in the cloud (free)
1. Make a free GitHub account, create a new repository, and upload everything in this folder
   (including the hidden .github folder).
2. Open the repo's Actions tab, pick "Build Plugg Lab", click Run workflow.
3. When it finishes (about 10 minutes), download the artifact for your OS. The .vst3 is inside.
