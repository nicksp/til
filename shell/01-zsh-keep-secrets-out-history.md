# Keeping secrets out of your ZSH history

I'm a big fan of zsh because of the power and customization it gives you.

One nice little trick I learned is that you can prevent commands from being added to your history by prepending a space to the line. This is useful for preventing any kind of secret, such as an API key, from being saved.

Just add `setopt HIST_IGNORE_SPACE` to your `.zshrc` and you're good to go :-)
