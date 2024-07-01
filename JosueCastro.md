We begin by initiliazing two variables : Start and Stop times.
We make a constant variable (final) which is nano seconds. 

The moment we do System.nanoTime(), (using System object we're already familiar with)
we are telling Java to begin counting the seconds this app is running for. 
It prints it in nano seconds.

We declared two methods, start() and stop() and they correspond 
with their respective Start and Stop times we created earlier. 

Now it gets more tricky.
We create a time() method. This will output the time the app has been running in seconds.
First we do StopTime minus StartTime. 
Why?
Because if StartTime doesnt start at 0, we won't know how much time has elapsed.
By doing StopTime minus StartTime we get the exact duration of how much time has passed since 
the timer went on and off.
And then at the end we divide it by NanosPerSec because there are 1000000000.0 nano seconds in one second.
ta-da! we have our elapsed time in seconds.

there is a toString() method to give a clean display to the user about how much time has passed in seconds. 
easy.

now we include a timeInNanoseconds method which is much simpler because we are already
in long nanoseconds units. so its simply return : (stoptime - starttime) and we know the elapsed time.

