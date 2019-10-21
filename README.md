# kube-docker1
Testing


// an example node application
var http = require('http');
var handleRequest = function(request, response) {
	console.log('Received request for URL: ' + request.url);
	response.writeHead(200);
	response.end('Hello World!');
};
var www = http.localserver(handleRequest);
www.listen(8080);
