This is a docker image that installs the latest [weechat](https://weechat.org) from the official repositories and the required dependencies for [wee-slack](https://github.com/rawdigits/wee-slack).

It makes no attempt to configure it as it is expected that you mount your configuration under ``/weechat/.weechat``.  I expose the relay on port 9080 and run the container interactively under tmux, the container runs on Europe/London time and with en_GB.UTF-8 -- because thats where I am.

``docker run -p 9080:9080 -v ~/.weechat:/weechat/.weechat --name weechat -ti adamgibbins/weechat``
