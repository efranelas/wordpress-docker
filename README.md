# wordpress-docker

WordPress application running inside a docker container.

If you prefer nginx over apache, you may want to clone [this repo](https://github.com/efranelas/wordpress-nginx-docker) instead.

# Instructions

1. After cloning this repository, create your `.env` file following the example stated in file `.env.example`.
```
cp .env{.example,}
```
Set your credentials and other needed variables in the file.

2. Start the containers:
```
docker-compose up -d
```

Access `http://localhost:8000` in your web browser to see your fresh new wordpress application running as a container.

PS.: The containers will create two folders in order to persist data. See the structure explanation below:

 - `.mysql` - MySQL Data Directory
 - `src` - The WordPress application source

