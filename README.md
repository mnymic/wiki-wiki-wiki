# foreach cycle to patch *.lnk for win+x menu
`gcis = gci; foreach ($gci in  $gcis) {hashlnk.exe $gci}`

# m-dot dotfiles
 **`net user administrator /active: yes`**

**```$obj = new-object -com wscript.shell; Sleep 7200; $obj.SendKeys([char]173)```**

## Install choco, set os

```New-Item -Path $profile -Type File -Force; get-content -path "$env:HOMEPATH\Documents\toolkit-bundle-dotfiles\pwsh\profiling\profile2022.ps1" > $PROFILE```

```Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'));choco install git -y```


```$toolkitPath = "$env:HOMEPATH\Documents\toolkit-bundle-dotfiles"; cd "$env:HOMEPATH\Documents"; git clone https://github.com/mnymic/toolkit-bundle-dotfiles.git; cd $toolkitPath; .\set-os.ps1```


# Config files
## vlcrc
 - $env:APPDATA\vlc\vlcrc
 - ~/.config/vlc/vlcrc

## dblcmd
$env:APPDATA\doublecmd\doublecmd.xml

## vimrc
https://github.com/amix/vimrc

`:e $MYVIMRC`

`:echo $MYVIMRC`

`~/.vimrc`

```source $VIMRUNTIME/vimrc_example.vim```

C:\tools\vim\_vimrc


## vifm
https://vifm.info/cheatsheets.shtml
see pngs in repo 4 chtsheets

`:echo $MYVIFMRC`

[https://github.com/vifm/vifm/blob/master/data/vifmrc]

## vlcrc
 - %appdata%\vlc\vlcrc

  ```cat $env:USERPROFILE\AppData\Roaming\vlc\vlcrc > $env:USERPROFILE\Documents\toolkit-bundle-dotfiles\#configs\vlcrc-backup```
  ```cat $env:USERPROFILE\Documents\toolkit-bundle-dotfiles\#configs\vlcrc > $env:USERPROFILE\AppData\Roaming\vlc\vlcrc```
 - ~/.config/vlc/vlcrc


## Win+x menu

```C:\Users\[USERNAME]\AppData\Local\Microsoft\Windows\WinX ```

## bash profile import
``` . /mnt/c/Users/$USERNAME/Documents/toolkit-bundle-dotfiles/nix/get-bashrc.sh```

``` cat /mnt/c/Users/$USERNAME/Documents/toolkit-bundle-dotfiles/nix/.bashrc > ~\.bashrc ```

## REGISRTRY PATHS

```Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Policies\System```

```Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\ShellCompatibility\InboxApp```

```Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders```

```Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\Explorer```

```Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Control Panel```

```Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion```

```Computer\HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System```

```Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\StuckRects3```
