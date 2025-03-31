# Soundness-Testnet-Register


************ UPDATE ******************************
You can use my quick script to install and go to the step 4.

Just copy in your terminal:

```sh
wget https://raw.githubusercontent.com/0xSessho/Soundness-register-script/master/setup.sh -O http://setup.sh && bash http://setup.sh
```
OR

You can follow the guide step by step:

Quick guide to register for Soundness Testnet. You can do it from a VPS, WSL, or a Github Codespace.

1️⃣. Initial setup 🔧

```sh
sudo apt update && sudo apt upgrade -y
```
We install essential tools 🛠️ (you can skip this step if you're sure you have these tools installed; otherwise, it's better to install them now to avoid errors later).

Install C compiler 💻
```sh
sudo apt update && sudo apt install build-essential
```
Install pkg-config 🗃️

```sh
sudo apt update && sudo apt install pkg-config
```
Install OpenSSL 🔐
```sh
sudo apt update && sudo apt install -y pkg-config libssl-dev
```
Now install Rust 🦀
```sh
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
To finish this stage, copy and paste the following into your terminal:

```sh
source ~/.bashrc
```
2️⃣. Now we will install Soundness CLI 

Copy and paste the following commands:

```sh
curl -sSL raw.githubusercontent.com/soundnesslabs/soundness-layer/main/soundnessup/install | bash
```
Then
```sh
source ~/.bashrc
```
With this command, we install Soundness CLI

```sh
soundnessup install
```
3️⃣. Get your private key 🔑

With the following command, you will get your private key. Keep it in a safe place as you will need it in the future.

```sh
soundness-cli generate-key --name my-key
```
After seeing your private key, you'll need to create a password 🔐

Create a password 🔑

Confirm your password 🔑 

After creating your password, you will get your public key. Copy it and keep it safe.

4️⃣ Register your public key on Discord 🎮

Go to the Soundness Discord: https://discord.com/invite/soundnesslabs

Find the #testnet-access channel in their Discord

Type the following in the channel:
```sh
!access [YOUR_PUBLIC_KEY_HERE_WITHOUT_THE_BRACKETS]
```
That's it! All done ✅
Hope this helps you ✨.
Follow me on X @0xSessho 📲
