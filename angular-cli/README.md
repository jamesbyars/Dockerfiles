# The Angular-CLI 

## Build

- Building the container `docker build -t angular-cli .`

## Run

- Run it `docker run -it -p 4200:4200 angular-cli bash`
- Create a new project `ng new PROJECT_NAME`
- `cd PROJECT_NAME`
- `npm install`
- `ng serve --host 0.0.0.0 --port 4200`
- See [angular-cli](https://github.com/angular/angular-cli) for other commands

## Mount a host directory 

`docker run -it -p 4200:4200 -v $(pwd):/home angular-cli bash`

## Tag & Push

1. Run Docker build (make sure to pass `-t angular-cli`)
2. `docker tag angular-cli jbyars4ku/angular-cli:[version]`
3. `docker push jbyars4ku/angular-cli:[version]`
4. `docker tag angular-cli jbyars4ku/angular-cli:latest`
5. `docker push jbyars4ku/angular-cli:latest`