### Welcome to Masonite

The [official](https://docs.masoniteproject.com/) documentation.

In order to install masonite, create a virtualenv and install with pip. I use windows for this repo.

``` bash
virtualenv msnite
.\msnite\Scripts\activate
pip install masonite
```

You will need version 3.6 of python and latest OpenSSL in order to use it.

Once the installation is complete you have to issue the **craft** command.

You should see a list of available commands in there.


``` bash
c:\users\dszabo\desktop\msnite\msnite\lib\site-packages\hupper\compat.py:2: DeprecationWarning: the imp module is deprecated in favour of importlib; see the module's documentation for alternative uses
  import imp
Masonite Version: version 3.0.12

USAGE
  Masonite Version: [-h] [-q] [-v [<...>]] [-V] [--ansi] [--no-ansi] [-n] <command> [<arg1>] ... [<argN>]

ARGUMENTS
  <command>              The command to execute
  <arg>                  The arguments of the command

GLOBAL OPTIONS
  -h (--help)            Display this help message
  -q (--quiet)           Do not output any message
  -v (--verbose)         Increase the verbosity of messages: "-v" for normal output, "-vv" for more verbose output and
                         "-vvv" for debug
  -V (--version)         Display this application version
  --ansi                 Force ANSI output
  --no-ansi              Disable ANSI output
  -n (--no-interaction)  Do not ask any interactive question

AVAILABLE COMMANDS
  help                   Display the manual of a command
  install                Installs all of Masonite's dependencies
  new                    Creates a new Masonite project
```

Let's create our first project.

``` bash
mkdir 1
cd 1
craft new
```

Once the project is ready we can start to serve our app with **craft serve** command and visit [localhost](http://127.0.0.1:8000/) to see the results.

Something like this.

![Logo](/Pictures/welcome.PNG)


Topics:

* [Creating a blog](/Guides/CreatingBlog.md)