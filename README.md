Quickstart
===============================================================================
* If you already have *make*, *rebar* and *git* in your path (even on windows)
    * make && ./startit
    * run whatever app you want by starting it -> helloworld:start()
    * check it out at http://localhost:8080
* *NOTE:* Apps all run on :8080 (so must be run one by one)

What is this?
===============================================================================
This is a simple project to show some examples of using the Erlang Cowboy 
"Small, fast, modular HTTP server and socket acceptor pool".  The first
order of business was to port all the amazing misultin examples over to 
cowboy.  Part of my motivation for doing this was the misultin end of 
life.

What isn't this? 
===============================================================================
This isn't documentation, or intended as any sort of documentation replacement
this is just a small set of working example you can run locally and quickly.

Too complicated?
===============================================================================
I did my best to keep it simple while following the OTP structure.  If you are 
un-familiar with OTP some of the examples might seem overly wordy.  I am not 
going to worry too much about that and just label it "bonus learning"! 

Each application was designed as an island able to be run completely seperate 
from the other applications (but obviously still has dependancies on cowboy).

Examples List
===============================================================================
* echo\_get -> Dealing with querystring data
* echo\_post -> Dealing with posted data
* hello\_world -> Start here! 
* hello\_world\_chunked -> Shows serving a reply in chunks
* hello\_world\_rest -> Show the RESTful upgrade / handler in Cowboy
* hello\_world\_ssl -> Show the simpliest SSL app
* redirect -> Show a basic redirect using a header
* static -> Show the static handler in Cowboy

Links
===============================================================================
* Cowboy -> https://github.com/extend/cowboy
* Cowboy Examples -> https://github.com/extend/cowboy_examples
* Webmachine (what Cowboy REST clones) -> http://wiki.basho.com/Webmachine.html
* Misultin -> https://github.com/ostinelli/misultin
* Misultin Examples -> 
  https://github.com/ostinelli/misultin/tree/master/examples
* Misultin End of Life -> 
  http://erlang.org/pipermail/erlang-questions/2012-February/064389.html

TODO
===============================================================================
* Access Log -> Hard to do right now due to lack of a good place to hook
* Comet
* Compression -> Coming soon, but will be hand coded 
* Cookies
* EventSource
* File (binary save)
* Multiple Servers (concurrently)
* Sessions
* Stream
* Websocket
