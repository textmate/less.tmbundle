# Installation

You can install this bundle in TextMate by opening the preferences and going to the bundles tab. After installation it will be automatically updated for you.

# Image Drop Action
Dragging an image into a LESS file will result in base64 data getting inserted into variables. The original idea was inspired by [this article about "Including Data URI Base64 encoded images easily (in LESS)"](https://github.com/cloudhead/less.js/wiki/Include-Data-URI-Base64-encoded-images-easily)

For example;

  Dragging and dropping "hamburger.png" onto a LESS file produces:
  
    @gfx-hamburger: "data:image/png;base64,[data]=";
    @gfx-hamburger-width: 79px;
    @gfx-hamburger-height: 90px;
    
  Which can be used thusly:
  
    background-image:url(@gfx-hamburger);
    background-size:@gfx-hamburger-width @gfx-hamburger-height;
    

# License (MIT)

Copyright (c) 2010 Scott Kyle and Rasmus Andersson

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
