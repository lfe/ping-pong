# LFE (Lisp Flavored Erlang) Example Application

This is an example of how you can use LFE to code Erlang OTP applications.

## Background Information

Read more about LFE @
  * http://github.com/rvirding/lfe
  * http://groups.google.com/group/lisp-flavoured-erlang
and Erlang / OTP @
  * http://www.erlang.org/doc

## Example Usage

This example assumes that you have installed LFE globally.

    $ ./rebar compile
    $ erl -pa ebin
    Eshell V5.7.3  (abort with ^G)
    1> application:start(ping_pong).
    ok
    2> ping_pong:ping().
    {pong,1}
    3> ping_pong:ping().
    {pong,2}
    4> ping_pong:ping().
    {pong,3}
    6> q().

As you can see it's not much - just a couple hours hacking, but it proves it
works and you don't have to code in erlang syntax to get erlang vm awesome
sauce.

## License

Copyright (c) Tim Dysinger tim <[<-on->]> dysinger.net

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
