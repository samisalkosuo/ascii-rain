# ascii-rain

Comfy rain for your console written in C with Ncurses.

<p align="center">
  <img src="https://github.com/nkleemann/ascii-rain/blob/master/demo/rain.gif" width="53.6%" height="40%"/>
  <img src="https://github.com/nkleemann/ascii-rain/blob/master/demo/rain_ho.gif" width="27%" height="100%"/>
</p>


## Dependencies 

You'll need a ncurses library. 

For Ubuntu packages are:

- 'ncurses-dev' or 'libncurses-dev'.

For OSX try:

- `brew install ncurses`.

For Linux (Rocky Linux 8.4 at least):

- `dnf -y install ncurses*`

## Build & Install

## AUR

You can get it from the AUR right [here](https://aur.archlinux.org/packages/ascii-rain-git/).

## Manual

- Clone this repo.
- Compile and link rain:
  - `gcc rain.c -o rain -lncurses`
- Compile and link rain (no color check):
  - `gcc rain-no-c-check.c -o rain -lncurses`
- Compile and link color demo:
  - `gcc color-demo.c -o color-demo -lncurses`

Now you can run 'rain' in your current working directory by just executing: ` ./rain`.

If you want to be able to run this program from every directory you have to copy the executable to `/usr/local/bin` or `/usr/bin`:
- `cp rain /usr/local/bin/rain`

## Notes & Troubleshooting

You'll (Or better, ncurses) need/s a somewhat modern terminal emulator with color support and the ability to hide the
cursor. Working examples are:

- iTerm 2 (OSX)
- OSX Terminal
- xfce4-terminal
- terminator

