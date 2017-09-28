# ProPresenter-OBS

Uses the ProPresenter Stage Display network API to feed current slide text into a vMix text input for lower thirds.

I happened upon this when the original author posted a link in a Facebook group. I figured I could tear it apart to use for OBS instead of the original vMix use. Please read through the comments in the code to see what info needs changed to match your environment.

Rename config.js.example to config.js and update the values to match your environment. In OBS, add a new BrowserSource, check "Local File", navigate to index.html, then set width, height, and FPS to match your stream settings. Edit stylesheet.css to customize your lower thirds setup.

Set the slide notes to `no-obs` on a slide to prevent it from being sent to vMix (useful for slides with more text than you would want in a lower third).
