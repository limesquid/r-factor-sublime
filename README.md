<div align="center">
  <a href="https://r-factor.org">
    <img src="https://raw.githubusercontent.com/limesquid/r-factor/master/logo.png" alt="R-Factor logo" />
  </a>

  <h1>R-Factor extension for Sublime Text 3</h1>

  <p>
    <img src="https://img.shields.io/github/package-json/v/limesquid/r-factor-sublime.svg" alt="Version" />
    <a href="https://github.com/limesquid/r-factor-sublime/blob/master/LICENSE">
      <img src="https://img.shields.io/github/license/limesquid/r-factor-sublime" alt="license" />
    </a>
  </p>

  <p>
    <a href="https://r-factor.org">Website</a> • <a href="https://r-factor.org/documentation">Documentation</a>
  </p>

  <hr />

  <p>
    <a href="https://github.com/limesquid/r-factor">R-Factor</a> • <a href="https://github.com/limesquid/r-factor-website">r-factor.org</a>
    <br />
    <a href="https://github.com/limesquid/r-factor-atom">Atom</a> • <a href="https://github.com/limesquid/r-factor-sublime">Sublime Text</a> • <a href="https://github.com/limesquid/r-factor-vscode">Visual Studio Code</a>
  </p>

  <hr />
</div>

## Install

### Stable version

```Shell
wget -c https://github.com/limesquid/r-factor-sublime/archive/refs/tags/1.0.1.zip -O r-factor-sublime.zip
mkdir -p ~/.config/sublime-text-3/Packages
unzip r-factor-sublime.zip -d ~/.config/sublime-text-3/Packages
rm r-factor-sublime.zip
mv ~/.config/sublime-text-3/Packages/r-factor-sublime-1.0.0 ~/.config/sublime-text-3/Packages/r-factor-sublime
cd ~/.config/sublime-text-3/Packages/r-factor-sublime
npm install
```

### Latest (master)

```Shell
wget -c https://github.com/limesquid/r-factor-sublime/archive/refs/heads/master.zip -O r-factor-sublime.zip
mkdir -p ~/.config/sublime-text-3/Packages
unzip r-factor-sublime.zip -d ~/.config/sublime-text-3/Packages
rm r-factor-sublime.zip
mv ~/.config/sublime-text-3/Packages/r-factor-sublime-master ~/.config/sublime-text-3/Packages/r-factor-sublime
cd ~/.config/sublime-text-3/Packages/r-factor-sublime
npm install
```

## Uninstall

```Shell
rm -rf ~/.config/sublime-text-3/Packages/r-factor-sublime
```

## Configure NODE_BIN

If `node` executable is not available in `PATH` env variable you might get `'NoneType' object is not subscriptable` error. In this case you need to manually set `NODE_BIN` path.

First, find out path to your node executable (e.g. `which node`).
Then, in Sublime go to "Preferences" -> "Package Settings" -> "R-Factor" -> "Settings - User", set `NODE_BIN` and save.

```json
{
  "NODE_BIN": "<<<<PASTE PATH TO NODE EXECUTABLE HERE>>>>"
}
```
