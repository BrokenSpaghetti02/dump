# Setting up Mini Pupper 1

### 1. Install python
```
sudo apt install -y git python3-pip
```
### 2. Clone the mini-pupper-2-bsp, only use the RPiCamera directory and install the camera module
```
cd ~
git clone https://github.com/mangdangroboticsclub/mini_pupper_2_bsp.git
cd mini_pupper_2_bsp/RPiCamera
./install.sh
rm -r mini_pupper_2_bsp/*
sudo reboot
```
### 3. Next, clone the gemini-md-bot repo and install
```
cd ~
git clone https://github.com/mangdangroboticsclub/gemini-md-bot
cd gemini-md-bot
./install.sh
```
### 4. Copy env.sample to .env and then set your google api key path
```
cp env.example .env
```
### 5. You can try testing out each of the api's in the api directory
```
cd gemini-md-bot/api
python google_api.py
```
