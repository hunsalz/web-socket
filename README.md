[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/hunsalz/web-socket)

# \<web-socket\>

A [Polymer 2.0](https://www.polymer-project.org/2.0/) element to ease the use and configuration of [WebSockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket).

A live [Demo](https://hunsalz.github.io/web-socket) of \<web-socket\>.

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

* __auto__ = Auto set to true, the web-socket tries to establish a connection on first page load
* __url__ = The URL to which to connect
* __protocols__ = An optional property to provide a single protocol string or an array of protocol strings.
* __state__ = The current state of the WebSocket connection. Notifies about state changes:  [WebSocket.readyState](https://developer.mozilla.org/en/docs/Web/API/WebSocket#Ready_state_constants)
* __last-request__ = The most recent request made by this web-socket element.
* __last-response__ = The most recent response received by this web-socket element.
* __last-error__ = The most recent error received by this web-socket element. If any error occurred.
* __verbose__ = Enables verbose mode

## Run your own prototype WebSocket-Server without great effort

Almost all demo references uses *wss://echo.websocket.org/* as WebSocket-Server. If you search for a local alternative, you can get up and running in minutes with  [httpwebsockethandler](https://github.com/SevenW/httpwebsockethandler) by [SevenW](https://github.com/SevenW)
