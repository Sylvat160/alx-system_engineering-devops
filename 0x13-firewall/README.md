# Resources

## Read or watch:

- [What is a firewall](https://en.wikipedia.org/wiki/Firewall)

## More Info

As explained in the web stack debugging guide concept page, `telnet` is a very useful tool to check if sockets are open. You can use it to test connections to specific ports on a remote server. For example, to check if port 22 is open on the server `web-02`, you can run the following command:

```
sylvain@ubuntu$ telnet web-02.holberton.online 22
Trying 54.89.38.100...
Connected to web-02.holberton.online.
Escape character is '^]'.
SSH-2.0-OpenSSH_6.6.1p1 Ubuntu-2ubuntu2.8

Protocol mismatch.
Connection closed by foreign host.
sylvain@ubuntu$
```

In this example, the connection is successful, and it displays the message "Connected to web-02.holberton.online."

Now, let's try connecting to port 2222:

```
sylvain@ubuntu$ telnet web-02.holberton.online 2222
Trying 54.89.38.100...
^C
sylvain@ubuntu$
```

In this case, the connection does not succeed, so after some time, the process is terminated using `ctrl+c`.

This `telnet` technique can be used not only for this exercise but also in any debugging situation where two pieces of software need to communicate over sockets.

Please note that the school network filters outgoing connections using a network-based firewall, which means you might not be able to interact with certain ports on servers outside the school network. To test your work on `web-01`, please perform the test from outside the school network, such as from your `web-02` server. If you SSH into your `web-02` server, the traffic will originate from `web-02` and bypass the school's network firewall.

**Warning!**
Containers on demand cannot be used for this project due to Docker container limitations.

Take extreme caution when configuring firewall rules. For example, if you deny port 22/TCP and log out of your server, you will not be able to reconnect to your server via SSH, and recovery may not be possible. By default, when you install UFW, port 22 is blocked, so remember to unblock it immediately before logging out of your server.