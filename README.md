###I no longer maintain this repo.

# Coursera Video Downloader Bookmarklet

Acknowledgements first, this project is a fork of [christiangenco's](https://github.com/christiangenco) [repo here](https://github.com/christiangenco/Coursera-Video-Downloader-Bookmarklet) which in turn is an expansion of [a gist](https://gist.github.com/1989008) by [csabapalfi](https://gist.github.com/csabapalfi).

This bookmarklet adds functionality to [Coursera](http://coursera.org)'s Video Lectures page to download and organize multiple videos at once with curl.

 ![Screenshot of the Coursera Video Downloader Bookmarklet](https://github.com/shivanker/Coursera-Video-Downloader-Bookmarklet/raw/master/screenshots/coursera_videos_after_bookmarklet.png)

The bookmarklet generates bash code that can be entered directly into the command line and will download the selected videos sequentially. The videos are organized in the following structure:

    1. Introduction - Why Model?/
       1. Why Model?.mp4
       2. Intelligent Citizens of the World.mp4
       ...
    2. Segregation and Peer Effects/
    ...

## Use

1. <a name="step2"></a>Add the script in [bookmarklet.js](https://raw.github.com/shivanker/Coursera-Video-Downloader-Bookmarklet/master/bookmarklet.js) as a bookmark in your browser.

  ![Bookmarklet](https://github.com/shivanker/Coursera-Video-Downloader-Bookmarklet/raw/master/screenshots/bookmarklet.png)
* Navigate to the "Video Lectures" page of any Coursera course.
  ![Coursera Video Lectures](https://github.com/shivanker/Coursera-Video-Downloader-Bookmarklet/raw/master/screenshots/coursera_videos_page.png)
* Click the "Coursera Downloader" bookmarklet in your bookmarks bar. This will add checkboxes to each video and a command output section at the top of the page.
  ![Coursera Video Lectures After Bookmarklet](https://github.com/shivanker/Coursera-Video-Downloader-Bookmarklet/raw/master/screenshots/coursera_videos_after_bookmarklet.png)
* <a name="select_all"></a> Select the videos you wish to download.
* "Select all" and "copy" the generated bash code in the text area near the top of the page.
  ![Copy Bash Code](https://github.com/shivanker/Coursera-Video-Downloader-Bookmarklet/raw/master/screenshots/copy_code.png)
* On your machine, open a terminal and navigate to the location you'd like your videos downloaded to.
  ![cd to video download location](https://github.com/shivanker/Coursera-Video-Downloader-Bookmarklet/raw/master/screenshots/cd_to_folder.png)
* Paste the GIGANTIC command into your terminal and hit enter.
  ![Past in generated code](https://github.com/shivanker/Coursera-Video-Downloader-Bookmarklet/raw/master/screenshots/terminal.png)

Your selected videos will now be downloaded with the `curl` utility and organized as described above.

## Other Coursera Downloader Tools

* [coursera-dl](https://github.com/jplehmann/coursera) by [jplehmann](https://github.com/jplehmann): "Script for downloading Coursera.org videos and naming them." (python)
* [coursera_downloader.py](https://github.com/LoganDing/Coursera.org-Downloader) by [LoganDing](https://github.com/LoganDing/): "A python script to download lectures (videos and slides) from Cousera.org" (python)
* [Coursera-Video-Downloader-Bookmarklet](https://github.com/andrewgph/Coursera-Video-Downloader-Bookmarklet): Another fork of christiangenco's repo by [andrewgph](https://github.com/andrewgph) which replaces the copy and paste command with direct (parallel) download by the browser.
