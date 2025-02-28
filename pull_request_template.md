## What?
 
Briefly describe the changes introduced by this PR. Highlight the difference between the state before and after the changes. Max 2 sentences.
 
## Why?
 
Why are these changes necessary? Is there a specific stakeholder (PM, service, QA, devs, sales) who is driving the motivation for these changes?
 
## How?
 
A high level description of the implemented changes. Visual aid is always preferred (diagrams, plots, tables, etc...).

## Backout plan

Briefly describe how to revert the feature in case of failure/issue. If not possible to revert 
1. name the reason for why it is not possible
2. think of any other way to handle possible failures/issues

> [!TIP]
> Do not waste too much time on deriving a backout plan. Your gut feeling will tell you what to do and if a backout plan is neccessary and applicable.
 
## Testing
 
Proof (in the form of screenshots, videos, graphs, etc...) that this feature/bugfix/hotfix is working as described. Steps to be followed for replicating results.

> [!NOTE]
> You can upload videos to GitHub by dragging, copy&pasting or via the attachment 📎 menu.
> To save some storage on GitHub you can use the following command to compress and/or speed up the video
> ```
> ffmpeg -i input.mov -vcodec libx264 -crf 35 -vf "setpts=0.25*PTS" output.mp4
> ```
> - The `-crf 35` sets the [Constant Rate Factor][crf], which is a scale from 0-51 where 0 is loseless compression and 51 is the worst possible.
> - The `-vf "setpts=0.25*PTS"` is a [filter][pts] to speed/slow up/down the video, in this case `0.25*PTS` will speed up the video 4x and `2*PTS` would slow it down by half.
>
> Install ffmpeg on Ubuntu
> ```
> sudo apt install ffmpeg
> ```
>
> Install ffmpeg on Mac via homebrew
> ```
> brew install ffmpeg
> ```

[crf]: https://trac.ffmpeg.org/wiki/Encode/H.264
[pts]: http://trac.ffmpeg.org/wiki/How%20to%20speed%20up%20/%20slow%20down%20a%20video#setptsfilter
