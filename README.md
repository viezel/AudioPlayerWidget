# Audio Player Widget

A small widget for Appcelerator Titanium. Its main purpose is to play audio files and showing media controls.


![Alt text](/blob/master/audioplayer.gif?raw=true "Audio Player")

## How to use

### View:


```xml
<Widget id="audioPlayer" src="dk.napp.audioplayer"></Widget>
win.add(imageView);
```

### Controller:

```javascript
$.win.addEventListener('open', function() {
	$.audioPlayer.setUrl("http://urltofile.mp3");
});

$.win.addEventListener('close', function() {
	$.audioPlayer.dispose();
});
```

### Style:

	"#audioPlayer":{
		styles:{
			wrap: {
				width: "260dp",
				height: "100dp"
			},
			
			playStopBtn: {
				color: Alloy.CFG.clientMainColor
			},
			
			scrubBar: {
				tintColor: Alloy.CFG.clientMainColor
			}
			
		},
		playIcon: Alloy.Globals.icons.play,
		pauseIcon: Alloy.Globals.icons.pause
	}



## Changelog
 

**v.1.0**  

* Initial implementation. 


## Author

**Mads Møller**  
web: http://www.napp.dk  
email: mm@napp.dk  
twitter: @nappdev  


## License

    Copyright (c) 2010-2014 Napp ApS

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