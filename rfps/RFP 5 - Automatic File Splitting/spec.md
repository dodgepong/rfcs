# Automatic File Splitting


## Feature Summary

Allow users to choose to save recordings in split files instead of one monolithic file.


## Motivation

When recording video files in OBS Studio, files are saved as a single video file. This makes sense in the general case, but there are some situations where having one single file is awkward. For example:

* If a video is long and recording at very high quality, the file size could be unwieldy to work with, especially in a video editor. File operations could take a long time when being applied to an overly-large video file.
* Many users feel a peace-of-mind about recordings that have been split and are finalized in context of taking efforts to prevent a file from being corrupted for some reason. While recording to FLV/MKV can prevent issues or video file corruption in the event of an OBS crash, that file format is not often easy to work with, given the necessesity of the extra remux step. Splitting files would allow users to record directly in MP4 with measures taken to combat file corruption.
* While streaming and recording a live event, it can be useful to start transferring and working the the recorded version of the stream before the stream ends for archival purposes. The streamer could stop and restart the recording, but it's convenient to not need to touch OBS in order to access recording files that have already been closed are are not being written to.


## Request For Proposal

Submit a proposal explaining how you will implement this feature such that it meets the following requirements:

* Add a feature to OBS recording settings to automatically split files according to user-specified criteria
    * Users should have the ability to select whether the file should be split after a certain amount of time (e.g. 20 minutes), or when a file reaches a certain file size (e.g. 4 GB).
    * Split files should play back seamlessly when stitched back together using a video editor, or a tool like FFmpeg. There should be no skipped frames or skipped audio.
    * The feature should be disabled by default.
    * File formats that require finalization should finalize invisibly in the background and should not interrupt the OBS UI when the file is split.


## Bounty

There is a bounty for the implementation of this feature.

* **Amount:** $500
* **Status:** Accepting Proposals

You can learn more about the OBS Project Bounty Program [here]().


## Completion Criteria

You may collect the bounty when the following are true:

* You have submitted one more more pull requests that fully implement the feature as you proposed.
* Your proposal addresses all items listed in the "Request For Proposal" section.
* Your pull request(s) are reviewed, and you have responded to review comments within a reasonable time frame.
* Your pull request(s) are merged into the `master` branch of the appropriate `obsproject` repositories.


## Additional Information

Related idea from the OBS Ideas Page:
* https://ideas.obsproject.com/posts/111/add-a-split-file-feature

Related posts on the OBS Forums:
* https://obsproject.com/forum/threads/automatic-split-output-files.73788/
* https://obsproject.com/forum/threads/file-split-after-size.43707/