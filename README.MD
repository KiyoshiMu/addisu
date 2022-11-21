
## Prerequisite

**If you have installed any, please skip that one**

1. Install Node Js https://nodejs.org/en/download/

1. Install Git https://github.com/git-guides/install-git


### Open your terminal

1. Config Git

       git config --global credential.helper store

1. Install Hexo

       npm install hexo-cli -g

1. Clone this Repo

       git clone https://github.com/AddisuLash/addisulash.github.io.git

1. CD to the Repo folder

       cd addisulash.github.io

1. Install dependencies

       npm i
## How to Change the content

You can learn [how to write](https://www.markdownguide.org/basic-syntax/) in a few minutes.

Use any editor change the related following files. Recommend [VScode](https://code.visualstudio.com/download).


You can open the website locally. Change the content and check the result.

    hexo g && hexo s

### Home Bio

source\bio.md

### About

source\about\index.md

### Media

source\media\index.md

### Teaching

source\teaching\index.md

### Research

source\research\index.md

For more complex design change, please contact [kiyoshi0mu@gmail.com](mailto:kiyoshi0mu@gmail.com).

## Deploy
    
    hexo clean && hexo deploy
