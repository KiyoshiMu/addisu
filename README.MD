
## Prerequisite

**If you have installed any, please skip that one**

1. Install Node Js https://nodejs.org/en/download/

1. Install Git https://github.com/git-guides/install-git


### Open your terminal

1. Config Git

       git config --global user.name [YOUR USERNAME]
       
       git config --global user.email [YOUR EMAIL]

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
    
### How to change image size

#### Home page

Change the width in your `addisulash.github.io/themes/hexo-theme-cupertino/source/css/index.css` file

```css
img {
  ...
  width: 75%;
}
```

#### Article Page

Change the width in your `addisulash.github.io/themes/hexo-theme-cupertino/source/css/post.css` file

Add `width: 90%;` then change the width.

From
```css
.content p img,
.content .block-large img {
  border-radius: 10px;
}
```

To


```css
.content p img,
.content .block-large img {
  border-radius: 10px;
  width: 90%;
}
```

### How to add image

#### Solution 1

1. Upload image to a hosting place, e.g. [Google Drive](https://www.labnol.org/google-drive-image-hosting-220515) and get its URL. 

1. Follow the markdown syntax.

```markdown
![img](URL)
```

#### Solution 2 (may not work)

1. Put the image in local `addisulash.github.io/source/` folder.

1. Follow the markdown syntax. Here the URL will just be your image name, like *img.jpg*.

```markdown
![img](URL)
```

### How to change Home Page title size

It's somewhat difficult to change the title size in home page.

You can change its font size at

`themes/hexo-theme-cupertino/source/css/index.css`

For large screens, change

 ```css
 .hero .large {
    font-size: 4vw;
    ...
}
```

For small screens, change

 ```css
@media screen and (max-width: 800px) {
    .hero .large {
        font-size: 7vw;
        ...
    }
}
```

### Home Bio

`source\bio.md`

### About

`source\about\index.md`

### Media

`source\media\index.md`

### Teaching

`source\teaching\index.md`

### Research

`source\research\index.md`

For more complex design change, please contact [kiyoshi0mu@gmail.com](mailto:kiyoshi0mu@gmail.com).

## Deploy
    
    hexo clean && hexo deploy
