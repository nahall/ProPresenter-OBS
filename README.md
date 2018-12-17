# ProPresenter-OBS

Uses the ProPresenter Stage Display network API to feed current slide text into a OBS browser source lower third.

I happened upon this when the original author posted a link in a Facebook group. I figured I could tear it apart to use for OBS instead of the original vMix use. Please read through the comments in the code to see what info needs changed to match your environment.

In ProPresenter you must Enable Network and Stage Display App under preferences.  Set a password under Stage Display App.

Rename config.js.example to config.js and update the values to match your environment.  Use the port listed under Enable Network not the port under the Stage Display App. Use the password under Stage Display App.

In OBS, add a new browser source, check "Local File", navigate to index.html, then set width, height, and FPS to match your stream settings. Edit stylesheet.css to customize your lower thirds setup.

Set the slide notes to `no-obs` on a slide to prevent it from being sent to OBS (useful for slides with more text than you would want in a lower third).
