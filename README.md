#This is a http request tip!

## Use curl to send http request with your command line

Can be useful to try your endpoint and see the result return by your server.

###GET

get on the main page:

curl https://ancient-bayou-3544.herokuapp.com

```http
<html>
    <head>
        <title>yo</title>
        <link rel="stylesheet" href="style.css">
        <link href='http://fonts.googleapis.com/css?family=Raleway:300' rel='stylesheet' type='text/css'>
    </head>
    <body>
        <div id="bar"></div>
        <div id="quackPoster">
            <textarea id ='enterQuack' type="text" name="name" placeholder="Quack at me bro!" value=""></textarea>
            <button id='sendQuack'>Quack</button>
        </div>
        <div id="quax">
        </div>
    <script src="https://cdn.socket.io/socket.io-1.2.0.js"></script>
    <script src="script.js" type="text/javascript"></script>
    </body>
</html>
```

get on the endpoint /main of the application

curl https://ancient-bayou-3544.herokuapp.com/main

[{"quack":"tweet tweet","time":"Wed Jun 10 2015","userID":"18916138","id":"1433947517803","lat":"51.5295436","lon":"-0.0422576"},{"quack":"heyyyy","time":"Wed Jun 10 2015","userID":"52075859","id":"1433947774409","lat":"51.529505","lon":"-0.0423901"},{"quack":"Hi","time":"Wed Jun 10 2015","userID":"18916138","id":"1433947778433","lat":"51.5295554","lon":"-0.0422953"},{"quack":"Amazing! ","time":"Wed Jun 10 2015","userID":"52075859","id":"1433947801075","lat":"51.5295061","lon":"-0.0423824"},{"quack":"stop that","time":"Wed Jun 10 2015","userID":"18916138","id":"1433948619062","lat":"51.529551899999994","lon":"-0.04227210000000001"},{"quack":"Quackkk!!","time":"Wed Jun 10 2015","userID":"44677574","id":"1433948620911","lat":"51.5295463","lon":"-0.0422526"},{"quack":"gfdgdfsgsdfgdsfgsfdgdfgdgfsdg","time":"Wed Jun 10 2015","userID":"44677574","id":"1433948660000","lat":"51.529481999999994","lon":"-0.0423268"},{"quack":"stoooooooop","time":"Wed Jun 10 2015","userID":"18916138","id":"1433948662567","lat":"51.5295632","lon":"-0.042283799999999996"},{"quack":"quuuuac","time":"Wed Jun 10 2015","userID":"18916138","id":"1433949055882","lat":"51.5295457","lon":"-0.0422573"}]


###POST (and break the application)

curl --data "quack='a new quack' https://ancient-bayou-3544.herokuapp.com/main

application broken!

To avoid some weird information to be recorded in your database or applicatin you need to check the data on the server side and not only on the front-end!!







