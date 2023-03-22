# Basic Flask application

This is a basic flask application that runs with docker. To run the application, go to the root directory of the project and use the following commands :

```
docker build -t basic-flask-application .
docker run -p 8080:8080 basic-flask-application
```

Next, open your browser and navigate to [http://localhost:8080/](http://localhost:8080/), and you should see the output of your application. 

![Flask Hello World Application](https://i.imgur.com/LJFRJU8.png)

Have fun !
Author : Lucien Chemaly
