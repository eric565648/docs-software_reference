# tmux {#tmux status=draft}

Author: Niklas Stolz, Chen-Lung Eric Lu

We all knows that if one disconnect an ssh connection, all running ros node will terminate, and we are not able to re-connect to the specific ssh connection again. Here we introduce a tool that overcome the problem.

## Advantages of using tmux

One could re-connect to a session.

The running ROS nodes won't die even the ssh connection has broken.

It's possible to connect to a specific session from another terminal.

## Installation

On Ubuntu, install using:

    $ sudo apt install tmux

## Basic Usage

First, open an ssh connection to a remote machine.

    $ ssh username@hostname

Then, by simply type 'tmux', you could start a tmux session

    $ tmux

If you wanna re-connect to a session instead of starting a new one, type this

    $ tmux attach

Last, you can terminate all session by typing this

    $ tmux kill-server

## Documentation

For more detail usage, please look up the github site of tmux

See also:
[tmux](https://github.com/tmux/tmux/wiki)
