# Terminal Profile

My terminal profile.

## Installation

### Powershell

1. Install [Powershell](https://apps.microsoft.com/store/detail/powershell/9MZ1SNWT0N5D), [Windows Terminal](https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701) & [NerdFonts](https://www.nerdfonts.com/).
2. Install [Scoop](https://scoop.sh/).
   ```
   iwr -useb get.scoop.sh | iex
   scoop install curl sudo jq
   ```
3. Install [oh-my-posh](https://ohmyposh.dev/).
   ```
   Install-Module posh-git -Scope CurrentUser -Force
   Install-Module oh-my-posh -Scope CurrentUser -Force
   ```
4. Install [Terminal-Icons](https://github.com/devblackops/Terminal-Icons).
   ```
   Install-Module -Name Terminal-Icons -Repository PSGallery -Force
   ```
5. Install [z](https://github.com/rupa/z).
   ```
   Install-Module -Name z -Force
   ```
6. Install [PSReadline](https://github.com/PowerShell/PSReadLine).
   ```
   Install-Module -Name PSReadLine -AllowPrerelease -Scope CurrentUser -Force -SkipPublisherCheck
   ```
7. Install [fzf](https://github.com/junegunn/fzf) & [PSFzf](https://github.com/kelleyma49/PSFzf).
   ```
   scoop install fzf
   Install-Module -Name PSFzf -Scope CurrentUser -Force
   ```
8. Copy _default.omp.json_ to _%homepath%/.config/powershell_.
9. Add lines in _powershell/user_profile.ps1_ to the Powershell profile.