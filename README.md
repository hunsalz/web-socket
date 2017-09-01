# \<web-socket\>

A [Polymer 2.0](https://www.polymer-project.org/2.0/) element to ease the use and configuration of [WebSockets](https://developer.mozilla.org/en-US/docs/Web/API/WebSocket).

## Install dependencies and run the demo

*Prerequisites:*

[npm](https://www.npmjs.com/)
[bower](https://bower.io/)
[Polymer CLI](https://www.npmjs.com/package/polymer-cli)

1. Run bower install from the repo directory:

    bower install

2. Run the Polymer development server from the project directory:

    polymer serve --open

## Usage

```html
<web-socket auto
            url="[[url]]"
            state="{{state}}"
            last-request="{{request}}"
            last-response="{{response}}"
            last-error="{{error}}"
            verbose>
</web-socket>
```

## Run your own prototype WebSocket-Server easily

Almost all demos reference *wss://echo.websocket.org/* as demo WebSocket-Server. If you search for a local alternative then you can try [httpwebsockethandler](https://github.com/SevenW/httpwebsockethandler) by [SevenW](https://github.com/SevenW)
