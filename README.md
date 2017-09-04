# \<web-socket\>

A [Polymer 2.0](https://www.polymer-project.org/2.0/) element to ease the use and configuration of [WebSockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket).

[Demo](https://hunsalz.github.io/web-socket)

## Install dependencies and run the demo

*Prerequisites:*

* [npm](https://www.npmjs.com/)
* [bower](https://bower.io/)
* [Polymer CLI](https://www.npmjs.com/package/polymer-cli)

*Install & run*

1. Run bower install from the repo directory:

```
    bower install
```

2. Run the Polymer development server from the project directory:

```
    polymer serve --open
```

## Usage

```html
<web-socket auto
            url="{{url}}"
            protocols="{{protocols}}"
            state="{{state}}"
            last-request="{{request}}"
            last-response="{{response}}"
            last-error="{{error}}"
            verbose>
</web-socket>
```

The above example illustrates the usage of `<web-socket>` in a [Polymer](https://www.polymer-project.org) app.

Attributes explained:

1. __auto__ = Automatically connecting on page load
2. __url__ = URL of WebSocket-Server
3. __protocols__ =
4. __state__ = The current state of the WebSocket connection. Notifies about state changes:  [WebSocket.readyState](https://developer.mozilla.org/en/docs/Web/API/WebSocket#Ready_state_constants)
5. __last-request__ =
6. __last-response__ =
7. __last-error__ =
8. __verbose__ = Enables verbose mode

## Run your own prototype WebSocket-Server without great effort

Almost all demo references uses *wss://echo.websocket.org/* as WebSocket-Server. If you search for a local alternative, you can get up and running in minutes with  [httpwebsockethandler](https://github.com/SevenW/httpwebsockethandler) by [SevenW](https://github.com/SevenW)
