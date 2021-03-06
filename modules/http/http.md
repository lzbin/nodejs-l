- HTTP
    - http.STATUS_CODES
    - http.createServer([requestListener])
    - http.createClient([port], [host])
    - Class: http.Server
        - 事件 : 'request'
        - 事件: 'connection'
        - 事件: 'close'
        - Event: 'checkContinue'
        - 事件: 'connect'
        - Event: 'upgrade'
        - Event: 'clientError'
        - server.listen(port, [hostname], [backlog], [callback])
        - server.listen(path, [callback])
        - server.listen(handle, [callback])
        - server.close([callback])
        - server.maxHeadersCount
        - server.setTimeout(msecs, callback)
        - server.timeout
    - Class: http.ServerResponse
        - 事件: 'close'
        - response.writeContinue()
        - response.writeHead(statusCode, [reasonPhrase], [headers])
        - response.setTimeout(msecs, callback)
        - response.statusCode
        - response.setHeader(name, value)
        - response.headersSent
        - response.sendDate
        - response.getHeader(name)
        - response.removeHeader(name)
        - response.write(chunk, [encoding])
        - response.addTrailers(headers)
        - response.end([data], [encoding])
    - http.request(options, callback)
    - http.get(options, callback)
    - Class: http.Agent
        - new Agent([options])
        - agent.maxSockets
        - agent.maxFreeSockets
        - agent.sockets
        - agent.freeSockets
        - agent.requests
        - agent.destroy()
        - agent.getName(options)
    - http.globalAgent
    - Class: http.ClientRequest
        - Event 'response'
        - Event: 'socket'
        - 事件: 'connect'
        - Event: 'upgrade'
        - Event: 'continue'
        - request.write(chunk, [encoding])
        - request.end([data], [encoding])
        - request.abort()
        - request.setTimeout(timeout, [callback])
        - request.setNoDelay([noDelay])
        - request.setSocketKeepAlive([enable], [initialDelay])
    - http.IncomingMessage
        - 事件: 'close'
        - message.httpVersion
        - message.headers
        - message.rawHeaders
        - message.trailers
        - message.rawTrailers
        - message.setTimeout(msecs, callback)
        - message.method
        - message.url
        - message.statusCode
        - message.socket