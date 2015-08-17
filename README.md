# I’m using nginx 1.8

I have upgraded all my servers to use Nginx 1.8.  The only thing I had
to change was the IPv6 “listen” linesefore, I had this:

```
listen [::]:80;
```

Now, I have two listen lines:

```
listen 80;
listen [::]:80;
```

Remember, the options given to ./configure last time are easily found:

```
nginx -V
```

And, oh, a couple URLs:

http://nginx.org/en/download.html

http://nginx.org/en/linux_packages.html#stable

