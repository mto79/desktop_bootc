# DESKTOP BOOTC

Making an atomic desktop with the code [https://github.com/mto79/desktop](https://github.com/mto79/desktop_bootc)

Thanks to bootc and the associated tools, building a personalised desktop experience is no longer difficult.

This project utilises quay.io/fedora/fedora-bootc as the base image to create a customizable container for building my perosnal desktop.

## Repository structure
I tried to organise the repository for easy reading and maintenance. 
Files are stored in functional and well-defined directories, making them easy to find and understand their purpose and where they will be placed in the container image.

Each file follows a specific naming convention. For instance a file /usr/lib/credstore/home.create.admin is named as usr__lib__credstore__home.create.admin

### Folders:

- .github: Contains an example of GitHub action to build the container and publish the image
- scripts: Contains scripts to be ran from the Containerfile during building
- system: Contains files to be copied to /usr and /etc
- systemd: Contains systemd unit files to be copied to /usr/lib/systemd

## Reference:

https://github.com/sigulete/kde-bootc
