# xpanes {#xpanes status=draft}

Author: Niklas Stolz, Chen-Lung Eric Lu

If you are dealing with multiple machines (servers, Duckiebots, etc.), we recommended you a tool that make your work more efficient. Also, much cooler.

## Advantages of using xpanes

You can open ssh connection to multiple machines at once

You can run commands on multiple machines at once.

## Installation

On Ubuntu, install using:

    $ sudo apt install software-properties-common
    $ sudo add-apt-repository ppa:greymd/tmux-xpanes
    $ sudo apt update
    $ sudo apt install tmux-xpanes

## Basic Usage

With xpanes we can open multiple ssh connections at a time and give the same commands to multiple bot.

You could combine the usage of xpanes with tmux.

See:[](#tmux)

Let's assume thay we're connecting to **watchtower 01 02** which have username **mom**

    $ xpanes -c "ssh mom@watchtower{}" 01 02

After sending the command, you should see the window split into two, each of them contain a ssh connection.

From that point, you can type in every command simultaneously. You could also combine the usage with tmux by typing

    $ tmux

It'll new a tmux session. Or you could attach old session by

    $ tmux attach

## Documentation

For more detail usage, please look up the official repository of tmux-xpanes

See also:
[tmux-xpanes](https://github.com/greymd/tmux-xpanes)
