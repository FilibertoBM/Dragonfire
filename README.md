# Dragonfire

the open-source virtual assistant for Ubuntu based Linux distributions

![Dragonfire](https://raw.githubusercontent.com/DragonComputer/Dragonfire/master/docs/img/demo.gif)

<p align="center"><sup><i>Special thanks to Jassu Ilama for the beautiful 3D modelling and material design of this avatar.</i></sup></p>

<p align="center">
  <a href="https://github.com/DragonComputer/Dragonfire/releases/latest">
    <img alt="GitHub Latest Tag" src="https://img.shields.io/github/v/release/DragonComputer/Dragonfire?logo=GitHub&style=flat-square">
  </a>

  <img alt="GitHub Downloads" src="https://img.shields.io/github/downloads/DragonComputer/Dragonfire/total?logo=GitHub&style=flat-square">
  <img alt="GitHub Last Commit" src="https://img.shields.io/github/last-commit/DragonComputer/Dragonfire?logo=GitHub&style=flat-square">
  <img alt="GitHub Commit Activity" src="https://img.shields.io/github/commit-activity/m/DragonComputer/Dragonfire?logo=GitHub&style=flat-square">

  <a href="https://github.com/DragonComputer/Dragonfire/blob/master/LICENSE.txt">
    <img alt="GitHub License" src="https://img.shields.io/github/license/DragonComputer/Dragonfire?logo=GitHub&style=flat-square">
  </a>

  <a href="https://github.com/DragonComputer/Dragonfire/actions?query=workflow%3ALinter%20Checks">
    <img alt="GitHub Workflow Linter Checks Status" src="https://img.shields.io/github/workflow/status/DragonComputer/Dragonfire/Linter%20Checks?logo=GitHub&label=linter%20checks&style=flat-square">
  </a>

  <a href="https://github.com/DragonComputer/Dragonfire/actions?query=workflow%3AAutomated%20Tests">
    <img alt="GitHub Workflow Automated Tests Status" src="https://img.shields.io/github/workflow/status/DragonComputer/Dragonfire/Automated%20Tests?logo=GitHub&label=automated%20tests&style=flat-square">
  </a>

  <a href="https://github.com/DragonComputer/Dragonfire/actions?query=workflow%3APublish%20a%20Release">
    <img alt="GitHub Workflow Debian Build Status" src="https://img.shields.io/github/workflow/status/DragonComputer/Dragonfire/Publish%20a%20Release?logo=Debian&label=debian%20build&style=flat-square">
  </a>

  <a href="https://github.com/DragonComputer/Dragonfire/actions?query=workflow%3ADocker%20Build">
    <img alt="GitHub Workflow Docker Build Status" src="https://img.shields.io/github/workflow/status/DragonComputer/Dragonfire/Docker%20Build?logo=Docker&label=docker%20build&style=flat-square">
  </a>

  <a href="https://hub.docker.com/repository/docker/dragoncomputer/dragonfire">
    <img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/dragoncomputer/dragonfire?logo=Docker&style=flat-square">
  </a>

  <a href="https://dragonfire.readthedocs.io/en/latest/dragonfire.html#module-dragonfire.api">
    <img alt="Read the Docs" src="https://img.shields.io/readthedocs/dragonfire?logo=Read%20the%20Docs&style=flat-square">
  </a>

  <a href="https://codecov.io/gh/DragonComputer/Dragonfire">
    <img alt="Code Coverage (Codecov)" src="https://img.shields.io/codecov/c/github/DragonComputer/Dragonfire?logo=Codecov&style=flat-square">
  </a>

  <a href="https://codeclimate.com/github/DragonComputer/Dragonfire">
    <img alt="Code Climate Technical Dept" src="https://img.shields.io/codeclimate/tech-debt/DragonComputer/Dragonfire?logo=Code%20Climate&style=flat-square">
    <img alt="Code Climate Maintainability" src="https://img.shields.io/codeclimate/maintainability-percentage/DragonComputer/Dragonfire?logo=Code%20Climate&style=flat-square">
    <img alt="Code Climate Maintainability Score" src="https://img.shields.io/codeclimate/maintainability/DragonComputer/Dragonfire?logo=Code%20Climate&style=flat-square">
    <img alt="Code Climate Issues" src="https://img.shields.io/codeclimate/issues/DragonComputer/Dragonfire?logo=Code%20Climate&style=flat-square">
  </a>

  <a href="https://gitter.im/DragonComputer/Lobby">
    <img alt="Gitter Chat" src="https://img.shields.io/gitter/room/DragonComputer/Dragonfire?logo=Gitter&style=flat-square">
  </a>

  <a href="https://opencollective.com/dragonfire">
    <img alt="Open Collective Backers" src="https://img.shields.io/opencollective/backers/dragonfire?logo=Open%20Collective&style=flat-square">
  </a>

  <a href="https://twitter.com/DragonfireAI">
    <img alt="Twitter" src="https://img.shields.io/twitter/follow/DragonfireAI?label=Mention%20Now%20%40DragonfireAI&logo=Twitter&style=flat-square">
  </a>
</p>

<br>

Dragonfire goes through these steps for each one of your commands, respectively:

 - Search across the built-in commands and evaluate the algebraic expressions
 - Try to [Learn using Advanced NLP and Database Management Techniques](https://github.com/DragonComputer/Dragonfire/blob/master/dragonfire/learn.py)

<br>

Dragonfire uses [Mozilla DeepSpeech](https://github.com/mozilla/DeepSpeech) to understand your voice commands and [Festival Speech Synthesis System](http://www.cstr.ed.ac.uk/projects/festival/) to handle text-to-speech tasks.

Feel free to join [our Gitter chat room](https://gitter.im/DragonComputer/Lobby). You can also directly talk with Dragonfire herself via [her Twitter account](https://twitter.com/DragonfireAI).

#### Supported Environments

|                         |                                         |
|-------------------------|-----------------------------------------|
| **Operating systems**   | Linux                                   |
| **Python versions**     | Python 3.8.x (64-bit)                   |
| **Distros**             | Ubuntu 20.04                            |
| **Package managers**    | APT, pip                                |
| **Languages**           | English                                 |
| **System requirements** | preferably a [CUDA supported GPU](https://www.geforce.com/hardware/technology/cuda/supported-gpus), 2GB of free RAM   |
|                         |                                         |

### Installation

To run Dragonfire on a desktop Debian or Ubuntu system, either download the [latest release](https://github.com/DragonComputer/Dragonfire/releases/latest) (the `.deb` file) and install as follows:

```Shell
sudo dpkg -i dragonfire_1.1.1_amd64.deb
```


or clone the GitHub repository and run

```Shell
sudo make install
```

in the repository directory.

<sup><i>To install the dependencies, run `sudo apt-get -f install` right after the `dpkg -i` command. The installation will automatically download the pre-trained English model of Mozilla DeepSpeech (1.31 GB download size) and will place it under `/usr/share/dragonfire/deepspeech/models` directory. You can manually [download the model](https://github.com/mozilla/DeepSpeech/releases/download/v0.4.1/deepspeech-0.4.1-models.tar.gz) if you wish.</i></sup>

If you want to run Dragonfire on a server, you should install the Docker image (which does not install the huge
DeepSpeech model required for speech recognition):

```Shell
docker pull dragoncomputer/dragonfire
```

### Usage <a href="https://dragonfire.readthedocs.io/en/latest/dragonfire.html#module-dragonfire.api"><img src="https://media.readthedocs.com/corporate/img/header-logo.png" align="right" height="25px" /></a>

```
usage: dragonfire [-h] [-c] [-s] [-j] [-v] [-g] [--server API_KEY] [-p PORT]
                  [--version]

optional arguments:
  -h, --help            show this help message and exit
  -c, --cli             Command-line interface mode. Give commands to
                        Dragonfire via command-line inputs (keyboard) instead
                        of audio inputs (microphone).
  -s, --silent          Silent mode. Disable Text-to-Speech output. Dragonfire
                        won't generate any audio output.
  -j, --headless        Headless mode. Do not display an avatar animation on
                        the screen. Disable the female head model.
  -v, --verbose         Increase verbosity of log output.
  -g, --gspeech         Instead of using the default speech recognition
                        method(Mozilla DeepSpeech), use Google Speech
                        Recognition service. (more accurate results)
  --server API_KEY      Server mode. Disable any audio functionality, serve a
                        RESTful spaCy API and become a Twitter integrated
                        chatbot.
  -p PORT, --port PORT  Port number for server mode.
  --version             Display the version number of Dragonfire.
```

or with Docker: `docker run dragonfire [-h] [-c] [-s] [-j] [-v] [-g] [--server API_KEY] [-p PORT]`

or simply start from your Linux application launcher.

<br>

To activate Dragonfire say *DRAGONFIRE* or *HEY* or *WAKE UP*.

To deactivate her say *GO TO SLEEP*.

To silence her say *ENOUGH* or *SHUT UP*.

To kill her say *GOODBYE* or *BYE BYE* or *SEE YOU LATER* or *CATCH YOU LATER*.

<br>

:warning: Facing with a problem? Take a look at the [Troubleshooting](https://github.com/DragonComputer/Dragonfire/blob/master/docs/TROUBLESHOOTING.md#troubleshooting):hammer_and_wrench: section.

<br>

#### Built-in Commands

[Dragonfire DEVLOG #3 - Built-in Commands](https://youtu.be/krHUzY2DylI)

```
DRAGONFIRE | WAKE UP | HEY
GO TO SLEEP
ENOUGH | SHUT UP
WHO AM I | SAY MY NAME
MY TITLE IS LADY | I'M A LADY | I'M A WOMAN | I'M A GIRL
MY TITLE IS SIR | I'M A MAN | I'M A BOY | CALL ME *
WHAT IS YOUR NAME
WHAT IS YOUR GENDER
FILE MANAGER | OPEN FILES
OPEN (BROWSER | CHROME | FIREFOX)
PHOTOSHOP | PHOTO EDITOR
INKSCAPE | VECTOR GRAPHICS
VIDEO EDITOR
OPEN [CAMERA, CALENDAR, CALCULATOR, STEAM, BLENDER, WRITER, MATH, IMPRESS, DRAW, TERMINAL]
SOFTWARE CENTER
OFFICE SUITE
KEYBOARD *
ENTER | NEW TAB | SWITCH TAB | CLOSE | GO BACK | GO FORWARD
SCROLL LEFT | SCROLL RIGHT | SCROLL UP | SCROLL DOWN
PLAY | PAUSE | SPACEBAR
SHUT DOWN THE COMPUTER
GOODBYE | BYE BYE | SEE YOU LATER
(SEARCH|FIND) * (IN|ON|AT|USING) WIKIPEDIA
(SEARCH|FIND) * (IN|ON|AT|USING) YOUTUBE
(SEARCH|FIND) * (IN|ON|AT|USING) (GOOGLE|WEB)
(SEARCH IMAGES OF|FIND IMAGES OF|SEARCH|FIND) * (IN|ON|AT|USING) (GOOGLE|WEB|GOOGLE IMAGES|WEB IMAGES)
WHAT'S THE TEMPERATURE IN *
WHAT TIME IS IT
```

<br>

#### Learning examples

[Dragonfire DEVLOG #4 - Learning](https://youtu.be/ujmRtqf2nxQ)

|                                                                 |                                                                  |
|-----------------------------------------------------------------|------------------------------------------------------------------|
| **You:** `THE SUN IS HOT`                                       | **You:** `MY PLACE OF BIRTH IS TURKEY`                           |
| **Dragonfire:** `OK, I GET IT. THE SUN IS HOT`                  | **Dragonfire:** `OK, I GET IT. YOUR PLACE OF BIRTH IS TURKEY`    |
| **You:** `THE SUN IS YELLOW`                                    | **You:** `WHERE IS MY PLACE OF BIRTH`                            |
| **Dragonfire:** `OK, I GET IT. THE SUN IS YELLOW`               | **Dragonfire:** `YOUR PLACE OF BIRTH IS TURKEY`                  |
| **You:** `DESCRIBE THE SUN`                                     | **You:** `YOU ARE JUST A COMPUTER PROGRAM`                       |
| **Dragonfire:** `THE SUN IS HOT AND YELLOW`                     | **Dragonfire:** `OK, I GET IT. I'M JUST A COMPUTER PROGRAM`      |
| **You:** `MY AGE IS 25`                                         | **You:** `WHAT ARE YOU`                                          |
| **Dragonfire:** `OK, I GET IT. YOUR AGE IS 25`                  | **Dragonfire:** `I'M JUST A COMPUTER PROGRAM`                    |
| **You:** `WHAT IS MY AGE`                                       | **You:** `ALBERT EINSTEIN IS A PHYSICIST`                        |
| **Dragonfire:** `YOUR AGE IS 25`                                | **Dragonfire:** `OK, I GET IT. ALBERT EINSTEIN IS A PHYSICIST`   |
| **You:** `FORGET MY AGE`                                        | **You:** `WHO IS A PHYSICIST`                                    |
| **Dragonfire:** `OK, I FORGOT EVERYTHING I KNOW ABOUT YOUR AGE` | **Dragonfire:** `ALBERT EINSTEIN IS A PHYSICIST`                 |
|                                                                 |                                                                  |

<br>

### Contribute

If you want to contribute to Dragonfire then please read [this guide](https://github.com/DragonComputer/Dragonfire/blob/master/CONTRIBUTING.md#contributing-to-dragonfire).
