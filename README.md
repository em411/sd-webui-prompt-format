# SD Webui Prompt Format
This is an Extension for the [Automatic1111 Webui](https://github.com/AUTOMATIC1111/stable-diffusion-webui), which helps formatting prompts.

<p align="center"><img src="Demo.jpg" width=512></p>

> The above demo was achieved in just 1 process

Sometimes, when you type too fast or copy prompts from all over the places, you end up with duplicated **spaces** or **commas**. This simple Extension helps removing them whenever you click **Generate**.

## Feature List
- [x] Works in both `txt2img` and `img2img`
- [x] Remove duplicated **spaces** and **commas**
- [x] Fix misplaced **brackets** and **commas**
- [x] Toggle `Remove Duplicates` to remove identical tags found in the prompts
  - **Note:** Only works for tag-based prompt, not sentence-based prompt 
    - **eg.** `1girl, solo, smile, 1girl` will become `1girl, solo, smile`
    - **eg.** `a girl smiling, a girl standing` will not be changed
- [x] Toggle `Remove Underscores` to replace `_` with **space**
  - *Some newer anime checkpoints claim to eliminate the need of using underscores*
- [x] Respect line breaks
  - **Note:** `Remove Duplicates` only checks within the same line
- [x] **[New]** Pressing `Ctrl + \` to quickly escape the **brackets** of the hovered tag
  - Normally, **brackets** *(parentheses)* are used to increase the weight of a prompt. Therefore, for tags like `mejiro mcqueen (umamusume)`, you will need to escape it like `mejiro mcqueen \(umamusume\)`.


<sup><b>Note:</b> This is purely visual. The actual prompt is unchanged until you manually edit the text again.</sup>