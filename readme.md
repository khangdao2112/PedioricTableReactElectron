# Periodic Table With ReactJS and ElectronJS
## About
This is our report submission for my Chemistry class (yeah learning chem in comp-sci no way). My PhD asked to do chemistry-related application or website for the report.  
To be honest with you I personally don't have much web development skill lol. So I resorted to the absolute classic

>**"If you can't do it, steal it"**  
>*- probably me -*  

Luckily I found this awesome Peridocic Table website using **ReactJS** by [Tamal Anwar Chowdhury](https://github.com/tamalchowdhury) (Please check him out I've been reading some of his articles recently and they're awesome). His implementation is simple but really easy to understand. Also through this project I've kinda grasped a bit of how ReactJS works.  
The real challenge here though is how do I get it to run as a program on my computer. This is where **ElectronJS** comes in. As I mentioned above I don't really have web-dev experience (I really mean it LOL I don't even know JavaScript) so throughout the process of transitioning his website to an actual app is really hard.
## The problem
You see normally ElectronJS would just run anything you put in `index.html` and then render it on the app window. But for React the outputs are all rendered code, so initially I pointed Electron to render my `localhost:3000` because React runs on port 3000. The problem is that you would have to start the web server first then launch Electron. This also caused problem to the build as well. So I had to redo the entire thing through this **Webpack** thing.  
After doing a bunch of stuff I was finally able to run both React and Electron on Runtime and in the build! (I'm too lazy to write them out lol)  
On the whole, I've learned a lot doing these stuff and I'm really happy that I got the desired outcome.
## Credits
- Big thank you to [Tamal Anwar Chowdhury](https://github.com/tamalchowdhury) and the original [Periodic Table website](https://github.com/tamalchowdhury/periodic-table)
- [Nguyen Thanh Khoi](https://github.com/khokhonguyen) for finding the upstream repo and some Front-end tweaks
- Me for:
    - Re-did some CSS styling and add some good looking fonts from Google Fonts
    - Implement Electron to build a fully fledged desktop app
## Running
### Prerequisites
- NodeJS (I'm using v19)
- Yarn (optional, you can use npm instead)
```bash
npm install --global yarn
```
### Run from source
- Clone this repository:
```bash
git clone https://github.com/laex2112/PedioricTableReactElectron.git
```
- Go to the new directory:
```bash
cd PedioricTableReactElectron
```
- Install dependencies:
```bash
yarn
```
- Run the app:
```bash
yarn start
```
### Build a distribution
```bash
yarn make
```
Your executable should be in `out\pediorictablereactelectron-win32-x64\pediorictablereactelectron.exe` and the installer should be in `out\make\squirrel.windows\x64\pediorictablereactelectron-1.0.0 Setup.exe`

## To-do
I might try to maintain and improve the app if I have free-time and the neccessary skills 🐧
- Improve UI
- Add more Element-related attributes available on the UI
