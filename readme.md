Clock
=====

Web based application showing the clock.

Usage with key control
-----

The following keys can be used to control the clock:

- `a` arms the clock to 2:30
- `s` starts or stops the clock
- `<space>` starts or stops the clock
- `x` stops the clock
- `[` reduces clock font size
- `]` increases clock font size

Usage with socketio
-----

Adjust the source to listen to a socketio stream

The clock listens to the following socketio messages

- `{cmd:'color',color:'#FF0000'}` sets the background color (for color keying purposes)
- `{cmd:'arm',countdown:30}` arms the clock (in this case 30 seconds, defaults to 2.5 min (150sec))
- `{cmd:'start',countdown:30}` arms the clock and starts it
- `{cmd:'stop'}` stops the clock
- `{cmd:'nudge',direction:'x',amount:10}` moves the clock in x or y direction by the given number of pixels
- `{cmd:'size',amount:2}` increases the font size by the given number of pixels

Open [clock.html](clock.html) on a system with google chrome web browser, set to full screen.