
# i3-alt-tab window switcher

Window switcher for i3

## Usage

Switch windows on the active/current workspace only.

~~~~sh
$ i3-alt-tab.py next current  # Focus next window in current workspace only
$ i3-alt-tab.py prev current  # Focus previous window in current workspace only
~~~~

Switch windows on all workspaces.

~~~~sh
$ i3-alt-tab.py next all  # Focus next window 
$ i3-alt-tab.py prev all  # Focus previous window
~~~~

## i3 configuration


### Bind alt+tab to switch windows in current workspace only.

Insert the following line into your i3 config;
~~~~
bindsym $alt+Tab exec i3-alt-tab.py next current
bindsym $alt+Shift+Tab exec i3-alt-tab.py prev current
~~~~

### Bind alt+tab to switch windows on all workspaces.

Insert the following line into your i3 config;
~~~~
bindsym $alt+Tab exec i3-alt-tab.py next all
bindsym $alt+Shift+Tab exec i3-alt-tab.py prev all
~~~~

