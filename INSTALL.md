# tut
https://www.youtube.com/watch?v=l2131Rok8XU&list=PLhHLdYJycWF--F2F7oMCiRWd8xNgIOUs4&index=40&t=15s

# docs & utilities
https://getbootstrap.com/

https://react-bootstrap.netlify.app/docs/getting-started/introduction

https://dummyimage.com/#google_vignette

https://picsum.photos

https://www.lipsum.com/

"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum."

# install

npm install react-bootstrap bootstrap

## App.js
```
import {Button} from 'react-bootstrap';
//import 'bootstrap/dist/bootstrap.min.css';
import '../node_modules/bootstrap/dist/css/bootstrap.min.css';
```

# docker
```
docker build . -t bs5-proto

docker network create microNetwork

# docker run --rm --name bs5-proto --network microNetwork -p 3000:3000 bs5-proto

docker run --rm --name bs5-proto -p 3000:3000 bs5-proto

# access docker shell
docker exec -it bs5-proto bash

# check exists
docker image ls
```

# gcloud deploy
```
gcloud builds submit --tag gcr.io/pfolio-deploy-1/bs5-proto

gcloud run deploy --image gcr.io/pfolio-deploy-1/bs5-proto --platform managed --port=3000
```