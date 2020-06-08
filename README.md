# FortunifAI - Responsive ComingSoon HTML Template
FortunifAI is a responsive, modern and clean under construction/coming soon template base on Bootstrap 3. This template is being packed with a countdown timer, ajax subscription form, social icons and about page.

FortunifAI comes in 4 versions: image background, Image Background + Countdown, Background Video and Background Image Slider.

FortunifAI have 5 color themes, green, red, yellow, blue and pink.

## Features
- Built on Bootstrap 3.2.0
- Fully Responsive
- Ajax Subscription form
- 5 Color themes
- FontAwesome icons
- Google Fonts
- Countdown
- Video Background
- Background Images Slider
- Displays well in all modern browsers and devices

## Component
### 1. Color Themes

To change color themes of button notify me, you have to choice from 5 color theme like Green, Red, Yellow, Blue, dan Pink.

```
<button type="submit" class="btn btn-notif green">Notify Me</button>
<button type="submit" class="btn btn-notif red">Notify Me</button>
<button type="submit" class="btn btn-notif yellow">Notify Me</button>
<button type="submit" class="btn btn-notif blue">Notify Me</button>
<button type="submit" class="btn btn-notif pink">Notify Me</button>
```

### 2. Email Subcribe

Open file sendmail.php find code :

```
$emailTo = 'your@email.com';
```
Enter the email where you want to receive the notification when someone subscribes.

#### 3. Images, Background images slide and Video Background

In FortunifAI pages you can have a static image, background images slide or a video as background.

#### A. For static image you have to change the url of this line.

```
<div class="main" style="background-image: url('images/bg.jpg')">
```

#### B. For background images slide you have to change 6 images of this line.

```
.cb-slideshow li:nth-child(1) span {
    background-image: url(../images/1.jpg)
}
.cb-slideshow li:nth-child(2) span {
    background-image: url(../images/2.jpg);
    -webkit-animation-delay: 6s;
    -moz-animation-delay: 6s;
    -o-animation-delay: 6s;
    -ms-animation-delay: 6s;
    animation-delay: 6s;
}
.cb-slideshow li:nth-child(3) span {
    background-image: url(../images/3.jpg);
    -webkit-animation-delay: 12s;
    -moz-animation-delay: 12s;
    -o-animation-delay: 12s;
    -ms-animation-delay: 12s;
    animation-delay: 12s;
}
.cb-slideshow li:nth-child(4) span {
    background-image: url(../images/4.jpg);
    -webkit-animation-delay: 18s;
    -moz-animation-delay: 18s;
    -o-animation-delay: 18s;
    -ms-animation-delay: 18s;
    animation-delay: 18s;
}
.cb-slideshow li:nth-child(5) span {
    background-image: url(../images/5.jpg);
    -webkit-animation-delay: 24s;
    -moz-animation-delay: 24s;
    -o-animation-delay: 24s;
    -ms-animation-delay: 24s;
    animation-delay: 24s;
}
.cb-slideshow li:nth-child(6) span {
    background-image: url(../images/6.jpg);
    -webkit-animation-delay: 30s;
    -moz-animation-delay: 30s;
    -o-animation-delay: 30s;
    -ms-animation-delay: 30s;
    animation-delay: 30s;
}
```
#### C. For the video background you need 2 video files (.webm and .mp4) and one image that represent the first frame of the video, in our case "bg-video.jpg".

```
 <div class="main" style="background-image: url('images/bg-video.jpg')">
        <video id="video_background" preload="auto" autoplay="true" loop="loop" muted="muted" volume="0">
            <source src="videos/sample.webm" type="video/webm">
                <source src="videos/sample.mp4" type="video/mp4">
                    Video not supported
        </video>
```
        
#### D. For countdown you have to change date of this line.

```
 $('#getting-started').countdown('2020/10/10').on('update.countdown', function (event) {
            var $this = $(this).html(event.strftime('' 
            + '<span>%-w</span> week%!w ' 
            + '<span>%-d</span> day%!d ' 
            + '<span>%H</span> hr ' 
            + '<span>%M</span> min ' 
            + '<span>%S</span> sec'));
});
```
