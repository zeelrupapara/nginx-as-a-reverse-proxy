# Use Nginx Reverse Proxy to serve Go and Nuxt Services

For understand Nginx implementation as a reverse proxy in different services like `Golang (as Api)` and `Nuxtjs (as Web)`

## Used Technology
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
![Go](https://img.shields.io/badge/go-%2300ADD8.svg?style=for-the-badge&logo=go&logoColor=white)
![Nuxtjs](https://img.shields.io/badge/Nuxt-002E3B?style=for-the-badge&logo=nuxtdotjs&logoColor=#00DC82)

## Installtion Requirement

| tool           | version |
|----------------|---------|
| `docker`         | *       |
| `docker-compose` | *       |

## Run Locally

Clone the project

```bash
  git clone https://github.com/zeelrupapara/nginx-as-a-reverse-proxy.git
```

Go to the project directory

```bash
  cd nginx-as-a-reverse-proxy
```

Install dependencies
  - go to the web directory

```bash
  cd web
```
- to install dependencies
```bash
  npm install
```

Run Locally using docker-compose
 - go back to project root
  ```bash 
  cd ..
  ```
- run project throw docker-compose
 ```bash
 docker-compose up
 ```
 After done all process see results in this link : `http://localhost:80/`
