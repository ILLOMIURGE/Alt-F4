---
author: Names of who wrote this post [optional, recommended]
editor: Names of who edited this post [optional]
translator: Names of who translated this post [optional]
image:
  url: Path to thumbnail for this ALT-F4 post (URI)
  transcription: Small transcription of the image thumbnail
title: Title of this ALT-F4 post
lang: en
discuss:
  forum: Link to forum thread [optional]
  reddit: Link to reddit thread [optional]
  discord: Link to discord chat [optional]
---

Welcome to this sample post, here we breafly describe how to use some advanced features of out templating configuration.

## Using Diagrams: [Mermaid](https://mermaid-js.github.io/mermaid/#/) <author></author>

You can create diagrams using Mermaid js. Please take look at full [documentation](https://mermaid-js.github.io/mermaid/#/) for more details

But here are some examples

You can use following code to create pichart
````
```mermaid !
pie title NETFLIX
         "Time spent looking for movie" : 90
         "Time spent watching it" : 10
```
````
```mermaid!
pie title NETFLIX
         "Time spent looking for movie" : 90
         "Time spent watching it" : 10
```

Or this code to create flow diagram
````
```mermaid !
graph TD
A[Christmas] -->|Get money| B(Go shopping)
B --> C{Let me think}
C -->|One| D[Laptop]
C -->|Two| E[iPhone]
C -->|Three| F[fa:fa-car Car]

```
````
```mermaid!
graph TD
A[Christmas] -->|Get money| B(Go shopping)
B --> C{Let me think}
C -->|One| D[Laptop]
C -->|Two| E[iPhone]
C -->|Three| F[fa:fa-car Car]

```

You can preview your diagrams [here](https://mermaid-js.github.io/mermaid-live-editor/#)

## Using Media <author></author>

You can use media by just importing it in a regular markdown fascion

1. Imgur
  - Use `![](https://i.imgur.com/WsUV4DK.gif)` or `{% include imgur.html id="WsUV4DK" %}`
  - where `id` is last part of Imgur URL https://imgur.com/gallery/`WsUV4DK`
  - ![](https://i.imgur.com/WsUV4DK.gif)
1. YouTube
  - `![](https://www.youtube.com/watch?v=dQw4w9WgXcQ)`
  - ![](https://www.youtube.com/watch?v=dQw4w9WgXcQ)


1. Dailymotion
  - `![](https://www.dailymotion.com/video/x7tfyq3)` or `![](https://dai.ly/x7tfyq3)`
  - ![](https://dai.ly/x7tgcev)

1. Vimeo
  - `![](https://vimeo.com/263856289)`
  - ![](https://vimeo.com/263856289)

1. Spotify
  - `![](http://open.spotify.com/track/4Dg5moVCTqxAb7Wr8Dq2T5)`
  - ![](http://open.spotify.com/track/4Dg5moVCTqxAb7Wr8Dq2T5)

1. SoundCloud
  - `![](https://soundcloud.com/aviciiofficial/preview-avicii-vs-lenny)`

1. General Audio
  - `![](//www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3)`
  - ![](//www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3)

1. Embeding a countdown
  - {% include countdown.html date="2021:01:01" %}
  - Where `date` is the date in year:month:day:hour:minutes:seconds, UTC



## Using Math: [MathJax](http://mathjax.org/) <author>Dr.MagPie</author>

You can use MathJax to describe mathematical equasions and formulas. You can find full specification in [MathJax Documentation](http://docs.mathjax.org/en/latest/) but here are come samples 

This code sample `$ a * b = c ^ b $` will transform into thes formula

$ a * b = c ^ b $

You can go full in and make some like this
```MathJax
$$
\begin{aligned}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{aligned}
$$
```
Which will look like this

$$
\begin{aligned}
  & \phi(x,y) = \phi \left(\sum_{i=1}^n x_ie_i, \sum_{j=1}^n y_je_j \right)
  = \sum_{i=1}^n \sum_{j=1}^n x_i y_j \phi(e_i, e_j) = \\
  & (x_1, \ldots, x_n) \left( \begin{array}{ccc}
      \phi(e_1, e_1) & \cdots & \phi(e_1, e_n) \\
      \vdots & \ddots & \vdots \\
      \phi(e_n, e_1) & \cdots & \phi(e_n, e_n)
    \end{array} \right)
  \left( \begin{array}{c}
      y_1 \\
      \vdots \\
      y_n
    \end{array} \right)
\end{aligned}
$$

You can preview your formulas [here](https://www.mathjax.org/#demo)