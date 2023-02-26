# Rclone Decrypt Express

Node.js Express based application that decrypts and visualizes directly in the browser a Rclone crypted file hosted in one of your remote instances (if it isn't possible to visualize the file in the browser, then it will be downloaded).

## Prerequisites

To use this codebase, you'll need the following installed on your system:

- [Node.js](https://nodejs.org/en/)
- [npm](https://www.npmjs.com/)

You also need a [Rclone](https://rclone.org/) crypted instance: a Blackblaze public bucket or similar cloud solutions are recommended for their ability to provide direct public download links, while for Google Drive or similar providers you should look on how to to get the direct public download link of one of your hosted files.


## Installation

- Open a terminal or command prompt.
- Clone this repository:
```bash
git clone https://github.com/Renzodef/Rclone-Decrypt-Express
```
- Navigate to the root directory of the cloned repository:
```bash
cd Rclone-Decrypt-Express
```
- Install the dependencies:
```bash
npm install
```
- Set the parameters of the file .env using your Rclone crypted instance password and salt: you can find them in the rclone.conf file as "password1" and "password2" in the section of your crypted instance.

## Usage
- Open a terminal or command prompt.
- Navigate to the root directory of this project.
- Start the server:<br>
```bash
npm start
```
- Open the browser (Chrome based browsers are recommended) and add to the base url of the service (localhost:3000 if you are trying in a local environment) the "fileUrl" parameter (the public download URL of one of your remote hosted Rclone crypted files):<br>
[http://localhost:3000/?fileUrl=your_file_url](http://localhost:3000/?fileUrl=your_file_url)
- To stop the server:<br>
```bash
npm stop
```