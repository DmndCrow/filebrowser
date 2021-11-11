# Filebrowser

Dropbox-like file manager, that can be set up on any server.

## Demo

![Demo](https://user-images.githubusercontent.com/5447088/50716739-ebd26700-107a-11e9-9817-14230c53efd2.gif)

## Prerequisites

Make sure you have installed these:
- [Docker and Docker Compose](https://phoenixnap.com/kb/install-docker-compose-on-ubuntu-20-04) - Will install all the required packages and software.


## Installation

Make a copy of `.env.example` file named `.env`

```shell script
cp .env.example .env
```

---

Environment variables:
- `UID` and `GID` - user and group, whose access will be used for this **Filebrowser** instance.
- `FB_PORT` - port on which the app will be running.
- `DOCKER_STATIC_HOSTING` - folder, that will be displayed.


```dotenv
# Docker settings
UID=0
GID=0
DOCKER_STATIC_HOSTING=/home/username
FB_PORT=8080
```

---

Build the Docker image

```shell script
docker-compose build
```

## Running

Start
```
docker-compose up
```

Stop
```
docker-compose down
```

## Usage

- Access **Filebrowser** instance through  `localhost:FB_PORT` from browser.
- Initial credentials are **login: admin** and **password: admin**
