# Discord-Bot
This is the code for our Discord bot which runs on our official Discord server at https://atl.pw/discord.

## Development
First things first you must have at least NodeJS 6.7.0. We highly recommend you use
[NVM](https://github.com/creationix/nvm) if on a unix like system as you can simply run `nvm use` in order to use the correct version of NodeJS.

Next clone this repo to a directory and then run `npm install` to install all the dependencies needed to run the bot.

Once installed you can run `npm run dev` to start the bot and auto reload when any changes are made to files.

## Building
To build this bot ready for running in production simply run `npm run build` which will compile all the files in the
*src/* directory and run it through Babel and spit it out in the *dist/* directory.

Once built simply run `npm run start` which will run the *index.js* file in the *dist/* folder.

## Docker
This repository contains support for Docker. Simply run `doceker build .` to build a Docker image ready to use.

Alternatively we have an automated build running on our Docker Hub repo at
https://hub.docker.com/r/atlauncher/discord-bot/

### Including secrets.json
In order to use the docker image, a secret.json must be provided at the */usr/src/app/config/* directory.

## Contributing
If you wish to contribute, please see the *CONTRIBUTING.md* file in the root of this repository.

## License
This code is licensed under the MIT license. For more details see the *LICENSE* file in the root of this repository.