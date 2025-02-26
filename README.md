<br />
<div align="center">
  <h3 align="center">Repo CC2 Linux</h3>

  <p align="center">
  	Commands and results
  </p>
</div>



<!-- CC2 -->
## Exercise 1

* find
  ```sh
  find -ctime 7 > Documents/recent_files.txt
  ```

* Output
  ```sh
  .
  ./.xsession-errors
  ./.sudo_as_admin_successful
  ./.bash_history
  ./Music
  ./.icons
  ./.icons/uwuntu-welcome.png
  ./Documents
  ./Documents/cc22.md
  ./Documents/cc2.md
  ./Documents/fileFromSevenDaysAgo
  ./Public
  ./.lesshst
  ./Desktop
  ./.Xauthority
  ./.profile
  ./Videos
  ./.bash_logout
  ./.config
  ./.config/fish
  ./.config/fish/functions
  ./.config/fish/functions/fish_greeting.fish
  ./.config/fish/config.fish
  ./.config/fish/completions
  ./.config/fish/conf.d
  ./.config/fish/conf.d/omf.fish
  ./.config/fish/fish_variables
  .local/share/gnome-settings-daemon/input-sources-converted
  ./Downloads
  ./Templates
  ./Templates/LibreOffice Calc.ods
  ./Templates/LibreOffice Impress.odp
  ./Templates/MS Excel.xlsx
  ./Templates/LibreOffice Writer.odt
  ./Templates/LibreOffice Draw.odg
  ./Templates/Text File.txt
  ./Templates/MS Word.docx
  ./Templates/Empty File
  ./Templates/MS PowerPoint.pptx
  ./.bashrc
  ```  

* Command 
  ```sh
  cat Documents/recent_files.txt | grep Ubuntu
  ```
* Output
  ```sh
  none
  ```

* Command 
  ```sh
  cat Documents/recent_files.txt | grep uwuntu                                                                                                                                                                       1 (0.002s) < 10:- output :
  ```
* Output
  ```sh
  ./.icons/uwuntu-welcome.png
  ```

## Exercice 2

* Command
  ```sh
  mkdir -p projet/src projet/bin projet/doc
  mv src/main.c src/util.c bin/ && mv src/util.h doc/
  tree
  ```
* Output 
  ```sh
  .
  ├── bin
  │   ├── main.c
  │   └── util.c
  ├── doc
  │   └── util.h
  └── src
  ```

## Exercice 3
* Commmand
  ```sh
  echo Data Confidential > secure_data/data.txt
  chmod 700 data.txt
  sudo chown thomas data.txt
  sudo setfacl -m u:aclTest:r data.txt
  ls -l
  ```
* Output
  ```sh
  total 4
  -rwxr-----+ 1 thomas baka 18 févr. 26 10:24 data.txt
  ```
* Command
  ```sh
  getfacl data.txt
  ```
* Output
  ```sh
  file: data.txt
  # owner: thomas
  # group: baka
  user::rwx
  user:aclTest:r--
  group::---
  mask::r--
  other::---
  ```


### Installation
_Below is an example of how you can instruct your audience on installing and setting up your app. This template doesn't rely on any external dependencies or services._

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/github_username/repo_name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```js
   const API_KEY = 'ENTER YOUR API';
   ```
5. Change git remote url to avoid accidental pushes to base project
   ```sh
   git remote set-url origin github_username/repo_name
   git remote -v # confirm the changes
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_

<p align="right">(<a href="#readme-top">back to top</a>)</p>




