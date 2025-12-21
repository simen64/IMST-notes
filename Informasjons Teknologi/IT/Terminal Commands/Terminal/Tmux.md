**Tmux** (Terminal Multiplexer) is basically a way to run _multiple terminal sessions inside one window._  You can:
- Split your terminal into panes (like a grid of mini terminals).

- Run multiple programs in the same window.

- Detach from your session (like closing the window) — and come back later to find everything still running.

You control Tmux with a prefix key which by deafault is ctrl + b. most commands would look like this:

**Commands**

Start tmux

	tmux

Detach 

	Ctrl+b then d

Reattach

	tmux attach

Create new window

	Ctrl+b then c

Switch window

	Ctrl+b then n or p

Split pane (horizontal)

	Ctrl+b then "

Split pane (vertical)

	Ctrl+b then %

Move Between panes 

	Ctrl+b then arrow keys

Close pane 

	exit or Ctrl+d


**Session Managment**

List sessions

	tmux ls

Create new named session

	tmux new -s mysession

Attach to session

	tmux attach -t mysession

Kill session

	tmux kill-session -t mysession

