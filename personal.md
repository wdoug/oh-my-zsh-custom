Here are a collection of a few other zshrc additions that I've ended up with over time:

```sh
# Personal config
# run nvm install if .nvmrc exists in opened directory (useful for vscode terminal)
[ -s "./.nvmrc" ] && nvm install

# Set up rupa z
# Move next only if `homebrew` is installed
if command -v brew >/dev/null 2>&1; then
	# Load rupa's z if installed
	[ -f $(brew --prefix)/etc/profile.d/z.sh ] && source $(brew --prefix)/etc/profile.d/z.sh
fi
```
