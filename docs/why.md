#Why do I need a plugin to test my bots?#
Bots are async in nature. 

In a very basic scenario, they work as APIs where a channel makes a `POST` to the Bot API, the Bot makes the processing and replies making another `POST` back to the channel. 

The image bellow shows how this works in practice:

[******* IMG *********]

This asynchronous nature makes hard to use tools like Apache JMeter, without a specialized toolkit like this one, to test Bot applications.

Using this tookit, we can capture the response sent by the bot by emulating a channel and with this approach we are able to measure the whole cycle from a request message to a response and have a clear view on the throughput the bot is capable of handling as well as the average, median and percentile latency the Bot is capable of.