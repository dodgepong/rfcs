# VST 3 Support


## Feature Summary

Allow users to use VST3 plugins as audio filters.


## Motivation

OBS Studio currently supports VST2 plugins. At the time when VST2 support was added, the VST3 SDK was not GPL-compatible, so we did not invest any time into including VST3 support when the feature was developed. Since then, Steinberg has released a GPL-compatible SDK for VST3, which now allows us to add support for VST3 plugins in public builds. Some VST plugins are VST3-exclusive, and often users of plugins that have both VST2 and VST3 versions released prefer to use the VST3 version.


## Request For Proposal

Submit a proposal explaining how you will implement this feature such that it meets the following requirements:

* Create a new plugin called `obs-vst3` that adds support for VST3 plugins
    * The plugin should be implemented on Windows, macOS, and Linux*
    * The plugin should use the Steinberg VST3 SDK directly instead of an intermediate library such as JUCE
    * The plugin should run VST3 plugins in an external process to avoid OBS crashing due to a VST plugin misbehaving
    * The plugin should search for VST3 plugins according to standard plugin location paths found in Steinberg documentation

\* Multiple contributors may assist with implementation on different platforms and may split the bounty according to the level of contribution they made to the project.


## Bounty

There is a bounty for the implementation of this feature.

* **Amount:** $2500
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
* https://ideas.obsproject.com/posts/75/add-vst-3-x-support
