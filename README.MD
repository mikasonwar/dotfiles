# Collection of personal dotfiles

First of all, hello and welcome!

I am currently mainly a ruby developer so you'll mainly find things tailored to that taste

Anyways here is the command to start using my dotfiles

```bash
cp -r ./neofetch_ascii ~/
cp .customrc ~/
cp .customps1 ~/
echo "source ~/.customrc" >> ~/.bashrc
echo "source ~/.customps1" >> ~/.bashrc
source ~/.bashrc
```

## Some points to consider:

- I like to keep my custom stuff in their own separate files so you'll find .customrc and .customps1 instead of a normal .bashrc
- I mainly use bash currently and i like to use neofetch to have a nice load screen
- Mainly use ubuntu + WSL
- I have ascii art popping up with neofetch, you can quickly add your own art just by dropping a file with the art in `~/neofetch_ascii`!
- I usually use RVM with my setup

Another thing i like to do is disable showing the package info with neofetch, as it pops up during every load of .bashrc it can become slow without it needing to be.

To do this you can `vim ~/.config/neofetch/config.conf` and delete the `info "Packages" packages`

## Some funcions I have setup

- `reload` - reloads the .bashrc, simple enough but a nice hack
- `quick_start` - starts things that I forget I need for the dev environment, currently it's postgres and redis!
- `code_bundle_show` - opens a vscode editor on the specified gem, for example if you type `code_bundle_show rails` it will open vscode editor on the local gem folder, pretty neat!