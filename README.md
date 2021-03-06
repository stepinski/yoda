<div align="center" style="margin: 20px">
  <img src="https://github.com/yoda-pa/yoda/raw/master/logo.png">
</div>

<div align="center">

  <h1>yoda</h1>
  <p>Wise and powerful personal assistant, inside your terminal</p><br>
  <a href="https://travis-ci.org/yoda-pa/yoda"><img src="https://travis-ci.org/yoda-pa/yoda.png" alt="Build status"></a> 
  <a href="https://sonarcloud.io/dashboard?id=yoda"><img src="https://sonarcloud.io/api/project_badges/measure?project=yoda&metric=alert_status" alt="SonarCloud Quality Status"></a> 
  <a href="https://manparvesh.mit-license.org/"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="License"></a> 
  <a href="https://github.com/yoda-pa/yoda"><img src="https://img.shields.io/badge/version-0.2.0-yellow.svg" alt="Project status"></a>
  
</div>


## Install, how to

#### Requirements

- [python (both 2 and 3 are supported)](https://www.python.org/downloads/)
- [virtualenv](https://virtualenv.pypa.io/en/stable/installation/) (only for testing and development)
- Python development package:
  - `python-dev` package (if using Ubuntu)
  - `Visual C++ 9.0 for Python` (If using Windows)
  - `python-devel` package (If using MacOS/OSX: [link](https://stackoverflow.com/questions/32578106/how-to-install-python-devel-in-mac-os/32578175#32578175))

### Run, how to

Clone this repository and create a virtual environment using Python 2 in the cloned directory (`virtualenv -p /usr/bin/python2 venv`). Steps after that:

![](https://raw.githubusercontent.com/yoda-pa/yoda/master/screencasts/firstsetup.gif)

Instead of `pip install --editable .` you can use `pip install .` if you don't intend to make any changes in the code.

## Use this package, how to

#### chat

This package contains a chatbot too! The `chat` command can be used to chat with it

![](https://raw.githubusercontent.com/yoda-pa/yoda/master/screencasts/chat.gif)

You can test the chat functionality on api.ai agent website [here](https://bot.api.ai/ff4ba99e-e444-4e19-8b4e-91fb0b93e414)

#### dev

This command group contains some sub-commands that may be helpful for developers and tech-geeks.

- speedtest

![](https://raw.githubusercontent.com/yoda-pa/yoda/master/screencasts/speedtest.gif)

- url

![](https://raw.githubusercontent.com/yoda-pa/yoda/master/screencasts/url.gif)

- hackernews

![](https://raw.githubusercontent.com/yoda-pa/yoda/master/screencasts/hackernews.gif)

#### diary

This command can be used to maintain a personal diary, roughly based on the concept of [Bullet Journal](http://bulletjournal.com/).

![](https://raw.githubusercontent.com/yoda-pa/yoda/master/screencasts/diary.gif)

#### love

This command can be used to maintain a profile of someone you love.

![](https://raw.githubusercontent.com/yoda-pa/yoda/master/screencasts/love.gif)

#### money

For tracking money, this is.

![](https://raw.githubusercontent.com/yoda-pa/yoda/master/screencasts/money.gif)

#### Idea list

For creating list of ideas, type

```
# To add idea
$ yoda ideas add --task <task_name> --inside <project_name>

# To show list of ideas
$ yoda ideas show

# To remove a task from idea
$ yoda ideas remove --task <task_name> --inside <project_name>

# To remove an idea completely
$ yoda ideas remove --project <project_name>
```

#### learn

This command group contains commands that, helpful in learning new things, will be.  Yeesssssss.

- vocabulary: For enhancing your vocabulary and tracking your progress.

    ![](https://raw.githubusercontent.com/yoda-pa/yoda/master/screencasts/vocab.gif)


- flashcards: for learning anything! ([inspiration](https://github.com/zergov/flashcards))

    ```
    # create new set (remember to keep the name to one word)
    $  yoda flashcards sets new english

    # modify set
    $  yoda flashcards sets modify english

    # list all sets
    $  yoda flashcards sets list

    # select a study set
    $  yoda flashcards select english

    # create new card in selected set (card name length can be more than 1 word)
    $  yoda flashcards cards new Oxford comma

    # Know which set is selected and its information
    $  yoda flashcards status

    # study the selected study set. This will show you all the cards in a study set
    # one by one.
    $  yoda flashcards study
    ```

- define: to get different meanings of a word. This definition search will be automatically saved, so that while you are working on your vocabulary, you can come through the new word as well.
![](https://raw.githubusercontent.com/yoda-pa/yoda/master/screencasts/define.gif)

#### Aliasing

This command group contains commands to alias cumbersome commands.

  ```
  # before: shortening a url
  $ yoda url shorten google.com
  
  # alias shorten to be s
  $ yoda alias new "shorten" "s"
  
  # can now use s in place of shorten
  $ yoda url s google.com
  
  # or alias the whole command as us
  $ yoda alias new "url shorten" "us"
  $ yoda us google.com
  
  # show your current aliases
  $ yoda alias show
  
  # delete aliases
  $ yoda alias delete "us"
  $ yoda alias delete "s"
  
  ```

#### feedback

To create an issue in the github repository simple thing that shows a link.  Yeesssssss.

![](https://raw.githubusercontent.com/yoda-pa/yoda/master/screencasts/feedback.gif)

## Packages and services used

- [Click](http://click.pocoo.org/5/): for building command line application
- [pychalk](https://github.com/anthonyalmarza/chalk): Colors in terminal
- [apiai](https://github.com/api-ai/apiai-python-client): api-ai for natural language understanding
- [pyyaml](https://pypi.python.org/pypi/PyYAML): for parsing yaml files
- [emoji](https://pypi.python.org/pypi/emoji/): emojis!
- [lepl](https://pypi.python.org/pypi/LEPL/): for formatted parsing
- [pycrypto](https://pypi.python.org/pypi/pycrypto): To encrypt / decrypt your password
- [pyspeedtest](https://pypi.python.org/pypi/pyspeedtest): To test network bandwidth
- [forex-python](https://pypi.python.org/pypi/forex-python): Foreign exchange rates and currency conversion
- [dulwich](https://github.com/jelmer/dulwich): for git
- [PyGithub](https://github.com/PyGithub/PyGithub): for using Github API v3
- [Gravit](https://gravit.io/): for creating the logo
- [chardet](https://github.com/chardet/chardet): universal character encoding detector
- [Codecov](https://codecov.io/): code coverage dashboard
- [coverage](https://pypi.org/project/coverage/): For code coverage testing
- [NumPy](http://www.numpy.org/): For scientific computation 
- [requests](http://docs.python-requests.org/en/latest/): For HTTP requests
- [nose](https://github.com/nose-devs/nose): For unit testing 
- [urllib3](https://github.com/urllib3/urllib3): HTTP client 
- [Certifi](https://github.com/certifi/python-certifi): Python SSL Certificates
- [idna](https://github.com/kjd/idna): For the domain name 
- [future](https://pypi.org/project/future/): the layer of compatability for Python 2/3
- [Google URL Shortener](https://developers.google.com/url-shortener/): URL shortener
- [News API](https://newsapi.org/): Used to get the top headlines from Hacker News
- [Forismatic API](https://forismatic.com/en/api/): Get random quotes that are used in the chat module
- [Cocktail DB](https://www.thecocktaildb.com/api.php): Used to search for a drink and to get a random drink
- [Words API](https://www.wordsapi.com/): Used to get the definition of a word
- Yoda's illustration SVG was taken from [here](https://www.shareicon.net/yoda-854796)

## Contribute, you must
Please refer to the [contributing guidelines](https://github.com/yoda-pa/yoda/blob/master/.github/CONTRIBUTING.md) for contributing to this project.

## In the news
- [ostechnix](https://www.ostechnix.com/yoda-the-command-line-personal-assistant-for-your-linux-system/)
- [sdtimes](https://sdtimes.com/os/sd-times-github-project-week-yoda-2/)
