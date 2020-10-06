{
  "Title": "mrpeek: a sixel-based terminal image viewer for MRtrix3",
  "issue_number": 202,
  "link_to_issue": "https://github.com/ohbm/hackathon2020/issues/202",
  "labels": [
    {
      "name": "EMEA hub",
      "description": "",
      "color": "b8aeef"
    },
    {
      "name": "Email ok",
      "description": "",
      "color": "bfdadc"
    },
    {
      "name": "Hackathon project",
      "description": "use this tag for submitted projects",
      "color": "fcffbc"
    },
    {
      "name": "Mrtrix",
      "description": "Using the Mrtrix software",
      "color": "6217b7"
    },
    {
      "name": "git-1",
      "description": "can commit and push to a repository",
      "color": "44ff44"
    },
    {
      "name": "unix command line",
      "description": "some knowledge of unix command line required",
      "color": "52e597"
    }
  ],
  "content": "**Guidelines**\r\n\r\n*We are very excited to meet you at the 2020 OHBM Brainhack \ud83c\udf89* *To submit a project, you need to be an attendee of the 2020 OHBM Brainhack. We ask you to register first over [here](http://www.humanbrainmapping.org/HackathonReg/). Thank you!*\r\n\r\n*We have prepared a checklist to help with your project submission. Here is how to proceed:*\r\n 1. *Before filling in any part, please submit this issue*\r\n 2. *Check items in the checklist below as you go through them*\r\n 3. *Once you are done (at least all 'required' items must be provided), please delete the \"Guidelines\" section add a comment saying 'hi @ohbm/project-monitors: My project is ready!'*\r\n\r\nThank you!\r\n\r\n*After step 1 (issue submitted), we will assign a 'project monitor' to follow your submission. If at any time you need help or anything is unclear, please add a comment and ping your project monitor. Our team is here to help!*\r\n\r\n\r\n----------------------------\r\n## Project info\r\n\r\n**mrpeek: a sixel-based terminal image viewer for MRtrix3**:\r\n\r\n**Project lead**: \r\n- J-Donald Tournier @jdtournier\r\n- Daan Christiaens @dchristiaens\r\n- Max Pietsch: @maxpietsch\r\n\r\n**[Timezone](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#timezone)**: London UTC+1\r\n\r\n**Hub**: Europe, Middle East and Africa\r\n\r\n**Description**:\r\n\r\nDisplaying images on a remote server is very difficult / impossible currently using [MRtrix3](https://www.mrtrix.org/)'s `mrview`, due the incompatibility of OpenGL 3+ with X11 forwarding ([see here for details](https://community.mrtrix.org/t/remote-display-issues/2547)). It will be some time before the technology is updated to fix this. \r\n\r\nIn the meantime, @wasserth's [niicat project](https://github.com/MIC-DKFZ/niicat) shows that it is possible to allow some (limited) display functionality using [sixel](https://en.wikipedia.org/wiki/Sixel). The [libsixel project](https://saitoha.github.io/libsixel/) provides an implementation that seems like a good starting point for a C++ command. \r\n\r\nThe aim of this project is to create a simple command for interactive display of MR images within the terminal, build on the [MRtrix3](https://www.mrtrix.org/) codebase, so that it can be used for quick inspection of images both locally and remotely.\r\n\r\nIf successful, changes will be included in a future update to the MRtrix3 software. [Contributors](https://github.com/MRtrix3/mrtrix3/blob/master/CONTRIBUTING.md) will be included in the built-in `git` [contribution statistics](https://github.com/MRtrix3/mrtrix3/graphs/contributors). We additionally credit contributors by showing their avatar at the bottom of the [_MRtrix3_ website front page](https://www.mrtrix.org/), and in the changelog as reported on the community forum ([example](https://community.mrtrix.org/t/mrtrix-3-0-rc3-3-0-0-changelog/3552)). \r\n\r\n**Link to project**: MRtrix3/mrtrix3#2079\r\n\r\n**Mattermost handle**: jdtournier\r\n\r\n**Goals for the OHBM Brainhack**\r\n\r\nThe range of possible milestones are presented in MRtrix3/mrtrix3#2079. The minimum requirements for the Hackathon would be: \r\n\r\n - extract a given slice of interest and render it to the terminal using libsixel\r\n- implement options or other user controls to select the slice of interest, projection (axial/sagittal/coronal), and brightness/control\r\n - implement real-time interaction based on keyboard input\r\n- implement real-time interaction based on mouse input\r\n\r\n**Good first issues**:\r\n\r\n- [Install MRtrix3 from source](https://mrtrix.readthedocs.io/en/latest/installation/build_from_source.html) and set up an [external linked module](https://mrtrix.readthedocs.io/en/latest/tips_and_tricks/external_modules.html) to create your own app\r\n- build a simple MRtrix3 app that can loop over a single slice of an image and extract the intensities (inspired by e.g. MRtrix3's [mrcolour](https://github.com/MRtrix3/mrtrix3/blob/master/cmd/mrcolour.cpp))\r\n- install [libsixel](https://saitoha.github.io/libsixel/) and add it as a dependency to your project (by editing your `config` file if needed)\r\n- work out how to feed the image intensities from the input data in a format suitable for [libsixel](https://saitoha.github.io/libsixel/), and display to the terminal\r\n\r\n**Skills**:\r\n\r\nSome experience with C++ is essential for this project. Experience with `git` and Unix in general would be advantageous. The pace of the project will however be tailored to the skillset of team members. No prior expectations are set on the quantity of team members.\r\n\r\n**Chat channel**: [hbmhack-mrpeek](https://mattermost.brainhack.org/brainhack/channels/hbmhack-mrpeek)\r\n\r\n**Video Channel** \r\n\r\nPlease have a look at the [Mattermost channel](https://mattermost.brainhack.org/brainhack/channels/hbmhack-mrpeek)(pinned posts) for the URL of the video channel, or alternatively, please contact to @jdtournier on Mattermost.\r\n\r\n\r\n**Image for the OHBM brainhack website**\r\n![84496961-344d7580-acae-11ea-91c1-e51971b1e7d5](https://user-images.githubusercontent.com/3221000/84586268-dfc20b80-ae0f-11ea-8129-d3e4e024caf9.png)\r\n\r\n## Project submission\r\n\r\n## Submission checklist\r\n*Once the issue is submitted, please check items in this list as you add under 'Additional project info'*\r\n\r\nPlease include the following above (all required):\r\n-   [x] Link to your project: could be a code repository, a shared document, etc. See [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#link-to-project)\r\n-   [x] Include your [Mattermost handle](https://mattermost.brainhack.org/) (i.e. your username). If you do not have an account, please [sign up here](https://mattermost.brainhack.org/signup_email).\r\n-   [x] Goals for the OHBM Brainhack: describe what you want to achieve during this brainhack. See [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#goals).\r\n-   [x] Flesh out at least 2 \"good first issues\": those are tasks that do not require any prior knowledge about your project, could be defined as issues in a GitHub repository, or in a shared document, cf [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#onboarding-2-good-first-issues).\r\n-   [x] Skills: list skills that would be particularly suitable for your project. We ask you to include at least one non-coding skill, cf. [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#onboarding-skills).\r\n-   [x] Chat channel: A link to a chat channel that will be used during the OHBM Brainhack. This can be an existing channel or a new one. We recommend using the [Brainhack space on mattermost](https://mattermost.brainhack.org/), cf. [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#chat).\r\n-   [x] Video channel: Please create a video channel that will be used during the OHBM Brainhack and share it in your chat channel above. This can be an existing channel or a new one. For instance a [jitsi meet](https://meet.jit.si/) room, cf. [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#video-calls).\r\n-   [x] Provide an image of your project for the OHBM brainhack website\r\n\r\nYou can also include information about (all optional):\r\n-   [x] Number of participants, cf. [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#participant-capacity)\r\n-   [ ] Twitter-size summary of your project pitch, cf. [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#twitter-size-summary-of-your-project-pitch)\r\n-   [ ] Set up a kanban board on your repository to better divide the work and keep track of things, cf [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#set-up-a-kanban-board)\r\n-   [ ] Project snippet for the OHBM Brainhack website, cf. [here](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#project-snippet-for-the-ohbm-brainhack-website)\r\n\r\nWe would like to think about how you will credit and onboard new members to your project. We recommend reading references from [this section](https://github.com/ohbm/hackathon2020/blob/master/.github/ISSUE_TEMPLATE/handbooks/projects.md#credit-and-onboarding). If you'd like to share your thoughts with future project participants, you can include information about (recommended):\r\n-   [x] Specify how will you acknowledge contributions (e.g. listing members on a contributing page).\r\n-   [ ] Provide links to onboarding documents if you have some.\r\n"
}