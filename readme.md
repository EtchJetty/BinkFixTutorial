# Using Bink 2.7 (Unreal) For Lagless Video Imports (FULL TUTORIAL)

To import a `.bik` format without lag, you can use either the original Bink 1 (less options, will have issues with colors, but you can skip the hex editing step) or Bink 2 (maximum compatibilty and options, requires extra steps outside of RAD Video Tools). 

If you already know how to prepare a file to be targeted by Bink, you can [skip ahead.](#bink-settings)

<details><summary><strong>Where to find Bink</strong></summary>
*Bink 1 can be found on the [RAD Video Tools site,](http://www.radgametools.com/bnkdown.htm), and Bink 2 is automatically included in downloads of [Unreal Engine 5.0.](https://docs.unrealengine.com/4.27/en-US/WorkingWithMedia/IntegratingMedia/BinkVideo/) You should be able to find Bink2ForUnreal.exe in even a partial download of the engine.*
</details>
<br />

## Video creation
Create whatever video you want, and decide on what animation you want it to replace (new animations entirely are out of scope for this tutorial, though with custom SJSON it is very much possible). In this tutorial, we'll be setting the Club Penguin Penguin's dance to be Zag's idle animation.

<p align="center">
![A gif of the Blue Penguin from Club Penguin dancing](https://file.garden/X8UcPOa95myVypAH/other/otherother/megido/pengdance.gif "Club Penguin Dance")
</p>

By going into `Hades/Content/Movies/`, we can find the `.bik` file that we want - `ZagreusIdle_Bink.bik`. It has a corresponding `.atlas.bik` file (contains the title of the bink file and some other data, but not important for a simple replacement).

Open `RAD Video Tools` or `Bink2ForUnreal.exe` and find your desired video! All screenshots in this tutorial will be using Bink 2, but the process is nearly identical in Bink 1.

![A screenshot of Hades' Content folder.](https://file.garden/X8UcPOa95myVypAH/other/otherother/megido/b1.png "Screenshot of Bink2ForUnreal")