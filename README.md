FlatBlue-css-theme-for-reddit
=============================

A subreddit theme to be used by subreddit owners on www.reddit.com

Icons thanks to Font Awesome http://fortawesome.github.io/Font-Awesome/

## Installation

[Grab the style from here](https://github.com/creesch/FlatBlue-css-theme-for-reddit)

Go to /r/<yoursubreddit>/about/stylesheet 

You'll find one text area where you can paste the css and below that options for uploading the images. 

**Upload the sprite images before saving the css**

That's about it for a basic installation.  

### css? 

If you haven't got the slightest clue as to what css is and how it works I really do recommend reading up on it. Even if you only plan to do some basic adjustments it helps a great deal if you have a basic grasp of the basics: 

- [Beginners guide to css](http://www.htmldog.com/guides/css/beginner/)
- /r/csshelp 

CSS in its most basic form is nothing more than saying "I want that thing with that name to have those properties". These things are called the box elements and that is basically what you are moving around with it. For example all the stuff on the sidebar on the right are in such an element which has the following name: 

      .side 

So if say for example you want to make the sidebar red you can do that like so


    .side { 
        background-color: red;
    }

Which is nothing more then pointing to the element, and then between the {} state what you want to do with it. 

### I still have trouble finding pages where I need to put it. 

Have a look at my ["Creating and moderating a subreddit 101"](http://www.reddit.com/r/creesch/wiki/mod101) guide. 


## Icons 
Icons are very simply to use, simply do the following 

    [](#icon-android)
Which will turn into [](#icon-android)
A complete list of the available icons can be found [here](/r/FlatBlue/w/icons) 

## Announcements 

In your sidebar simply put a triple quote and a h6 to turn it into an announcement. For example this sub has the following:

    >>> ###### Announcement [with a link](/r/boxed)


## Colored boxes in your sidebar

    ###### Red header
    >
    > Red box
    
    #### Green header
    >
    > Green box
    
    ##### Blue box
    >
    > Blue box

## Spoilers 

`[This is a spoiler](#spoiler)`     
[This is a spoiler](#spoiler)  

## Changing font sizes

With this theme it is no longer needed to search the entire css for all size declarations! Simply look for the one block of code that handles ***all*** font sizes. 

## Header size

When adjusting the header height you also will need to adjust some other positioning. For your convenience those lines of codes are positioned directly after the code for the header. 

## Required images

- header-blue.png 
- reddit-res-sprite-icons.png
- sprite-icon-32.png (white and dark versions are available)
- sprite-icon-16.png

## Link flairs

Link flairs couldn't be more easier. By default there are 7 premade colored flairs included which are alphabetically named starting from a and ending with g. Simply use those in the class field and you will see that each correspondents with a color. 

If you want to add more flairs look for the following line of code and follow the instructions: 

    /* not enough flairs?  Simply copy the following text and change <CLASS>  to whatever class you want to name the flair and <COLOR> to a valid hex color (#ff0000 for example)
