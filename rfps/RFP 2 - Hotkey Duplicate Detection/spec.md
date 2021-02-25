# Duplicate Hotkey Warning in Settings


## Feature Summary

Show a warning in the hotkeys settings panel if a key or key combination is in use by another hotkey shortcut.


## Motivation

Right now, OBS users are able to set multiple actions to the same shortcut. Frequently this can be intentional, as some users wish for OBS to be able to do multiple things with a single keypress. However, this is not always the case, and users may want to know when a hotkey they set is already in use so that they are fully aware of what might happen when the press that hotkey. Therefore, OBS should show a warning when a duplicate shortcut is set, but because we want to keep the ability to trigger multiple actions with the same shortcut, the warning should not be interruptive.


## Request For Proposal

Submit a proposal explaining how you will implement this feature such that it meets the following requirements:

* A visual warning is shown in the hotkeys settings panel when a hotkey is used by two or more items.
* Any text in the warning uses the Qt translated strings feature.
* The visual warning is not a pop-up/modal, nor is it interruptive. That is, it should not require user interaction to dismiss, nor should it be unnecessarily overbearing.


## Bounty

There is a bounty for the implementation of this feature.

* **Amount:** $200
* **Status:** Accepting Proposals

You can learn more about the OBS Project Bounty Program [here]().


## Completion Criteria

You may collect the bounty when the following are true:

* You have submitted one more more pull requests that fully implement the feature as you proposed.
* Your proposal addresses all items listed in the "Request For Proposal" section.
* Your pull request(s) are reviewed, and you have responded to review comments within a reasonable time frame.
* Your pull request(s) are merged into the `master` branch of the appropriate `obsproject` repositories.


## Additional Information

Initial proposal from OBS Ideas page: [https://ideas.obsproject.com/posts/1327/duplicate-hotkeys-warning](https://ideas.obsproject.com/posts/1327/duplicate-hotkeys-warning)
