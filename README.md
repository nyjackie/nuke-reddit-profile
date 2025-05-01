# nuke-reddit-profile
Scripts to nuke reddit profiles

Nuke Reddit Comments

```
# go to https://old.reddit.com/user/DunnoWhatKek/comments/
# run below script - this will delete all the comments on the current page

var i = 0;
var tags = document.querySelectorAll("form[class='toggle del-button '] > span > a[class='yes'] ")
	
window.setInterval(function(){
  tags[i].dispatchEvent( new MouseEvent(
        'click',
        { view: window, bubbles: true, cancelable: true }
    ));
	i++;
}, 1000);
```
