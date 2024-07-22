# Setting up Mini Pupper 1

### Make sure to update the system first and install python
```
sudo apt update
sudo apt upgrade
sudo apt install -y git python3-pip
```
### Clone the StanfordQuadruped repo and install
```
cd ~
git clone https://github.com/mangdangroboticsclub/StanfordQuadruped.git
cd StanfordQuadruped
./install.sh
```
### Then clone the mini_pupper_bsp repo and install
```
cd ~
git clone https://github.com/mangdangroboticsclub/mini_pupper_bsp.git
cd mini_pupper_bsp
./install.sh
```
### Next clone gemini-md-bot repo and install
```
cd ~
git clone https://github.com/mangdangroboticsclub/gemini-md-bot
cd gemini-md-bot
./install.sh
```
### Copy env.sample to .enc and then set your google api key path
```
cp env.example .env
```
### You can try testing out each of the api's in the api directory
```
cd gemini-md-bot/api
python google_api.py
```
