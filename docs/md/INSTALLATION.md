## Installation (MacOS) 

### Documents By Docsify
to use docsify:
```bash
# add global install of docisify
yarn global add docsify-cli 

# initialize docs folder with docsify files
docsify init ./docs
```
```bash
# command to display readme's in browser
docsify serve ./docs

# results
Serving /Users/jasmineanderson/Genspark/Projects/Humans-VS-Goblins/docs now.
Listening at http://localhost:3000
```

<!-- ### Features -->

### App module
0. Install Programs
    * Java
    * Gradle
    * Groovy
    * Jenkins

1. Clone Repository
```bash
https://github.com/jazicorn/Humans-VS-Goblins.git
```
2. Build Project
```bash
# [Folder] Command
[Humans-VS-Goblins] ./gradlew build
```
3. Run Project
```bash
# [Folder] Command
[Humans-VS-Goblins]  ./gradlew run
```

#### Dockerize Project
0. Install Docker
```bash
# homebrew install
brew install --cask docker
```
1. Build Docker Image
```bash
# [Folder] [Humans-VS-Goblins/product-app] 
docker build -t jazicorndev/hvsg.product-app . 
```
2. Run Docker Image
```bash
docker run -d -p 8081:8081 -e "SPRING_PROFILES_ACTIVE=dev" hvsg/product-app:latest 
```
5. Create DockerHub Account
   1. Sign up and create a free DockerHub account for personal use, if you don’t have one.
   2. Next, you login to your DockerHub account and create a repository with name and description for e.g. hvsg.product-app
   3. At this stage, our account and repository is created. We’re going to push the images to this remote repository using docker command that means our Docker Desktop should be running in our local machine.
   4. How to authenticate before pushing to remote repository? Go to Docker Desktop -> Images -> Remote Repositories, and Sign in with DockerId and password of your DockerHub account. Now all docker push commands will be authenticated automatically.
   5. Alternatively you can use following command to login, it will prompt for username and password: `docker login`
6. Tag Local Image to Remote Docker Image
```bash
docker tag hvsg/product-app:latest jazicorndev/hvsg.product-app/0.0.1
```
8. Push Repository with Tag
```bash
# [Folder] [Humans-VS-Goblins/product-app]
docker push jazicorndev/hsvg.product-app:latest  
```