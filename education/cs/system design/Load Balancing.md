
#### What is it?

Load balancing is an intermediary between client and server, it allows for the equal distribution of data to ensure no server becomes overloaded, and has constant uptime. This is achieved through distributing the data between other servers etc.

An example of this is 'round-robin', this is where the load balanced will distribute data by incrementing through the servers one at a time until it reaches the final one, at which point the loop will reset, this allows for each server to have even distribution of data.

Example: Google

Google handles load balancing in layers, they use one global IP address that routes users to a nearby data centre, this will then distribute data to a backend based on health, proximity, latency, and capacity. Allowing billions of searches with constant uptime.



