# scrollsnap
Pure CSS scrolling slide to next content.

Add this to your container

````
.container {
    -webkit-overflow-scrolling: touch;
    scroll-snap-type: mandatory;
    /* older spec implementation */
    scroll-snap-destination: 0% 100%;
    scroll-snap-points-x: repeat(100%);
}
`````

The snaping items should have this styling

`````
.item {
    scroll-snap-align: start;
}
`````

However this does not work on all devices. 
Tested only in Chrome.

[Pollfills](https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/scroll-snap-polyfill.js) are needed for this to work.

```````
https://s3-us-west-2.amazonaws.com/s.cdpn.io/4273/scroll-snap-polyfill.js
```````