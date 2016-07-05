croutonext\_server
------------------

A quick and dirty minimal websocket server to support crouton's chrome
extension. Just has basic support for setting the host's clipboard,
opening URLs, and sending desktop notifications.

Requires python 3.4 or later, click, and websockets.

Usage
-----
Run the server:
```
./croutonext_server
```

Set clipboard contents:
```
echo "foobar" | ./croutonext_client -
```

Open URL
```
echo "http://example.com" | ./croutonext_client --command U -
```

Send notification
```
echo '{"title":"Notify!", "message":"Message from chroot."}' | ./croutonext_client --command N -
```
