# Using Bink 2 (Bink2ForUnreal) For Lagless Video Imports in HADES (FULL TUTORIAL)

*(If you already know how to prepare a file to be targeted by Bink, you can [skip ahead to the Bink Settings.](#bink-settings))*


To import a `.bik` formatted video file into Hades without the lag that had previously stopped the community from replacing video files, you can use either the original RAD Video Tools (Bink 1; less options, will have issues with colors, but you can skip the hex editing step) or Bink2ForUnreal (Bink 2, maximum compatibilty and options, requires extra steps outside of RAD Video Tools, <span style="text-decoration: underline;">*recommended*</span>). This guide will be using Bink 2, though we'll cover Bink 1 options when relevant.

<details><summary><strong>Click For Links And Info On How to Download Bink 2 or 1 (free!)</strong></summary><blockquote><hr>
Bink 1 can easily be found for free on the <a href="http://www.radgametools.com/bnkdown.htm">RAD Video Tools site</a>, and Bink 2 is automatically included in downloads of <a href="https://docs.unrealengine.com/4.27/en-US/WorkingWithMedia/IntegratingMedia/BinkVideo/">Unreal Engine 5.0.</a> You should be able to find Bink2ForUnreal.exe in even a partial download of the engine. It can also be <a href="https://github.com/marcussacana/Bink2/raw/main/Bink2%20Encoder%20%2B%20DLLs%20FINALLY.rar">found elsewhere</a>, if need be.
<hr>
<h3>Bink 2 from Unreal Engine</h3>
<img src="docs/a2.png" alt="A screenshot showing that Bink2ForUnreal.exe is located in C://Program Files/Epic Games/UE_50./.egstore/bps/Install/Engine/Binaries/ThirdParty/Bink">

<h3>Bink 2 from Unreal Engine</h3>
<img alt="A gif of the Blue Penguin from Club Penguin dancing" src="docs/a1.png?raw=true" title="Club Penguin Dance">
<hr>
</blockquote>
</details>
<br />
<h2>Video creation</h2>
Create whatever video you want, and decide on what animation you want it to replace (new animations entirely are out of scope for this tutorial, though with <a href="https://github.com/SGG-Modding/SGG-Mod-Format/wiki/Import-Type:-SJSON">custom SJSON</a> it is very much possible). In this tutorial, we'll be setting the Club Penguin Penguin's dance to be Zag's idle animation.
<br /><br />
<p align="center">
<img alt="A gif of the Blue Penguin from Club Penguin dancing" src="https://file.garden/X8UcPOa95myVypAH/other/otherother/megido/pengdance.gif" title="Club Penguin Dance">
</p>

By going into `Hades/Content/Movies/`, we can find the `.bik` file that we want—`ZagreusIdle_Bink.bik`. It has a corresponding `.bik_atlas` file. 

> (The `.bik_atlas` file contains a header and the bink file's name and resolution. If keeping resolution and filename the same (<u>*recommended*</u>), the `.bik_atlas` file can be safely ignored. If changing resolution, skip ahead to [the bik_atlas](#understanding-the-bik-atlas), but understand that this is literally undocumented territory, and may be really annoying to work with.)

Open `RAD Video Tools` or `Bink2ForUnreal.exe` and find your desired video! All screenshots in this tutorial will be using Bink 2, but the process is nearly identical in Bink 1.

<div align="center"><img style="max-width: 50vw;"  alt="A screenshot of Hades' Content folder." src="docs/b1.png" title="Screenshot of Bink2ForUnreal"></div>
You'll want to navigate to your Hades folder (this will likely work for other Supergiant Titles, but this guide was written for Hades) and find its Content subfolder. If your 