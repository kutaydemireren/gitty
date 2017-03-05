This is an helper for installing gitignore.

** Easy, customizable, extendable. Set-up and be ready in 2 minutes, then waste just a second to create gitignore from now on. **

With this script, instead of looking and building a gitignore file up from scracth, at every beginning of a project, I simple use this bash script. That is I am also adding to here. 

It is seriously easy and simple. And the good thing with this is you can extend or customize as you wish since it is just a bash script after all. For example, if the cases are not enough for you, just add another by looking at the site https://github.com/github/gitignore. This is where my code looks for, eventually. 

Helps me a lot, hope it will help you too.

* Step by step Setup
  1) Simple enough, you just have to install this gitty script. Go to raw mode and download it. 
  2) Give it the right permissions which is executable and can be given by 'chmod +x gitty'.
  3) Turning it into a command, called gitty.
        For Linux users: add the file to your /usr/bin and now you are good to go 
        For Mac users: add the file anywhere you'd like - a suggestion is into /usr/local/ -, then open the file .profile (or .bash_profile, it varies depending on your system). Now write 'alias gitty='the-path-you-chose' without apostrophes.
  4) You are good to go :)

* Usage
  To download gitignore, as example case, if you want to download ruby, simply write gitty ruby. See the avaliable options from CASES array, at the beginning of the script.
  To update, type gitty update, and it will update by re-downloading the .gitignore you have.
    
* Customize / Extend
  Customizing cases:
     If you don't like gitty ruby but you want to write gitty r, you can do it! Open script, find CASES array; delete "ruby" and type back as "r". 
  Extending cases-results:
     If you want to add another gitignore other than those avaliable on the script itself, it is easy as well! Open script, find CASES and RESULTS arrays; (say you want to add CMake case), add into CASES array whatever you would like to call it, e.g. "cmake". Also add into RESULTS the corresponding, actual name of, gitignore file which are avaliable on https://github.com/github/gitignore, so in cmake example it would be "CMake". 

* Notes
  It create .gitty file when you download a gitignore. It is normal. It is necessary for the 'update' feature to work.

* Author
  Kutay Demireren

* Contribute
  Feel free to contribute in any way you would like. Pull request's are welcome.