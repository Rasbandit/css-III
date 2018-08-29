# Animations / Responsive

## Responsive Design
- start with space jam website
  - Show how beautiful the site isn't.
  - also show how how it would look on a phone.
  - This site was made when the only things that went to sites were monitors.

- Tinker Watches https://tinkerwatches.com/
  - Look at how clean this looks, but also see how it changes when we shrink it down.
  - The site looks drastically different and we even loose some animation that don't fit.
    - trend, more and more people are using mobile to browse the web, with as much as 25% doing mobile only.
    - So if you ignore mobile side then you could be losing a large majority of your user base.
    - we can see media queries using the debugger tool

- thought experiment, what is the resolution of an iphone 10? is it larger or smaller than a monitor?
    - It is 2436 x 1125, compared to the monitor in front of you that has 1920 x 1080,
      - hd is 2,073,600 pixels and an iPhoneX is 2,740,500. That is a 700,000 pixel difference.
    - show what a website would look like if that really was how phones showed web pages.
    - So how does an iphone really show off the site?
    - DPR, device pixel ratio.

- Extraxtion and Enchancement approaches.
  - not real industry terms
    - extraction is going desktop first then mobile, can be hard to squish it all in or take things out.
    - enchancemnet is starting mobile and going up.

- Conventional wisdom says to build for mobile first, aka Responsive Design.
  - Define responsive design
    - Responsive Web Design is about using HTML and CSS to automatically resize, hide, shrink, or enlarge, a website, to make it look good on all devices (desktops, tablets, and phones):
  - to do this we will be using media queries.
  - Before we can get into the meat we need to understand some things about css.

## CSS

- order matters, show how more recent item overwrites old one.
- so using this idea we can use what are called media queries to dynamically change the site.
  - Two big ones to use are min-width and max-width
    - min-width is for going phone to desktop
    - max-width is for going desktop to mobile
    - show how you can view these on chrome
    - https://www.w3schools.com/cssref/css3_pr_mediaquery.asp
  - media queries should be on the bottom
  - The keyword AND can be used to combine multiple queries
    - one additional nice MQ is screen orientation,
      - landscape and portrait

- Build bootstrap nav bar in react, so you can also show how to use react to make animations
  - https://blackrockdigital.github.io/startbootstrap-blog-post/
- show that

## Animations

- Animations on web pages can really take it up a level
  - http://www.theglyph.studio/#home
  - some are complex, some are simple.

- Over the top animations
  - https://www.lingscars.com/

- Transitions
  - use transitions to show animation in nav.
  - show how transitions can take 3 params, time, what transition, and the rate of change.
    - cubic bezier http://cubic-bezier.com/
  - w3 can tell you what properties can transition.

- Transistion is great for simple animations but not great for more complex animations
  - @keyframe is a way to really get some interesting animations
    - basic is from and to
    - more control uses %
  - lets make an animation loop toggleable in react

- React motion is a library that can do some cool things

## Animation Tags
@keyframes: Specifies the animation code
animation: A shorthand property for setting all the animation properties
animation-delay:Specifies a delay for the start of an animation
animation-direction:Specifies whether an animation should be played forwards, backwards or in alternate cycles
animation-duration: Specifies how long time an animation should take to complete one cycle
animation-fill-mode: Specifies a style for the element when the animation is not playing (before it starts, after it ends, or both)
animation-iteration-count: Specifies the number of times an animation should be played
animation-name: Specifies the name of the @keyframes animation
animation-play-state: Specifies whether the animation is running or paused
animation-timing-function: Specifies the speed curve of the animation