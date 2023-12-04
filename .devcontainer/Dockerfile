FROM mcr.microsoft.com/devcontainers/javascript-node:0-20

RUN apt-get update && export DEBIAN_FRONTEND=noninteractive

RUN sudo apt install apt-transport-https dirmngr gnupg ca-certificates
RUN apt-key adv --keyserver hkp://keyserver.ubuntu.com --recv-keys 3FA7E0328081BFF6A14DA29AA6A19B38D3D831EF
RUN echo "deb https://download.mono-project.com/repo/debian stable-buster main" | sudo tee /etc/apt/sources.list.d/mono-official-stable.list
RUN sudo apt-get update
RUN sudo apt-get install -y mono-complete
RUN sudo apt-get install -y wine

RUN npm update -g npm
RUN npm install -g electron-packager

