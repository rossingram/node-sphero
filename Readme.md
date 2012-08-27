# Node Sphero

## How to use

    npm install node-sphero

Connect your [Sphero](http://gosphero.com) to your laptop over bluetooth. At this time only OSX 10.8 has been tested.

Add Sphero to your app:

    var roundRobot = require('node-sphero');
    var sphero = new roundRobot.Sphero();

    sphero.connect();

    sphero.on("connected", function(ball){
      var rgb = color();
      sphero.setRGBLED(0, 255, 0, false);
    });

Run that, and your sphero should turn #00FF00... green.

Check out the examples for more ideas.


## API

TODO.. fill in this list...

setBackLED
setRGBLED
setHeading
roll

## In Progress

The rest of the sphero bluetooth api functionality.

## Thanks 

Awesome work by [Bradley Meck](https://github.com/bmeck) who built the initial version.
