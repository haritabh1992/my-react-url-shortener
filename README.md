# React app - URL Shortener

Created using [Create React App](https://github.com/facebook/create-react-app)

Also followed this [blog](https://mherman.org/blog/dockerizing-a-react-app/#production) sepcifically for the docker setup

Quick build command:
```
$ docker build -t sample:dev .
```

Quick spin up command:
```
$ docker run \
    -it \
    --rm \
    -v ${PWD}:/app \
    -v /app/node_modules \
    -p 3001:3000 \
    -e CHOKIDAR_USEPOLLING=true \
    sample:dev
```

Open your browser to http://localhost:3001/ and you should see the app. Try making a change to the App component within your code editor. You should see the app hot-reload. Kill the server once done.
