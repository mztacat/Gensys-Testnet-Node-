# Gensys-Testnet-Node-

### The Gensyn Protocol is a layer-1 trustless protocol for deep learning computation that directly and immediately rewards supply-side participants for pledging their compute time to the network and performing ML tasks.
-------------------

![image](https://github.com/user-attachments/assets/2b8f84fe-5581-4c69-abcc-b158a0f1922f)



# Requirements
---
Ensure you that you are using a supported machine/device/environment:

arm64 or x86 CPU with minimum 16gb ram
OR

### CUDA devices (officially supported):
- RTX 3090
- RTX 4090
- A100
- H100
- WITH

Python >=3.10 (for Mac, you will likely need to upgrade)

---
## Testnet participation
### Please answer 'Y' (or just press enter), N is provided as an alternative flow but isn't currently maintained.

 - Login
 - A browser window will pop open (you'll need to manually navigate to http://localhost:3000/ if you're on a VM).
 - Click 'login'.
 - Login with your preferred method.


## Setting up system 
```
sudo apt update && sudo apt upgrade -y
```

## Essenstials 
```
sudo apt install -y \
  curl \
  git \
  wget \
  nano \
  tmux \
  htop \
  nvme-cli \
  lz4 \
  jq \
  make \
  gcc \
  clang \
  build-essential \
  autoconf \
  automake \
  pkg-config \
  libssl-dev \
  libleveldb-dev \
  libgbm1 \
  bsdmainutils \
  ncdu \
  unzip \
  tar

```

## Installing python 
```
sudo apt-get install -y \
  python3 \
  python3-pip \
  python3-venv \
  python3-dev
```

## Node and Yarn 
```
sudo apt-get update && curl -fsSL https://deb.nodesource.com/setup_22.x | sudo -E bash - && sudo apt-get install -y nodejs && node -v && sudo npm install -g yarn
```


## Install Docker 
```
for pkg in docker.io docker-doc docker-compose podman-docker containerd runc; do
  sudo apt-get remove $pkg
done

sudo apt-get update
sudo apt-get install -y ca-certificates curl gnupg

sudo install -m 0755 -d /etc/apt/keyrings
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /etc/apt/keyrings/docker.gpg
sudo chmod a+r /etc/apt/keyrings/docker.gpg

echo "deb [arch=$(dpkg --print-architecture) signed-by=/etc/apt/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu $(. /etc/os-release && echo "$VERSION_CODENAME") stable" | \
sudo tee /etc/apt/sources.list.d/docker.list > /dev/null

sudo apt-get update
sudo apt-get install -y docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose-plugin

```





---
## Install Python & PIP 
```
sudo apt install python3 -y && sudo apt install python3-pip -y
```
![image](https://github.com/user-attachments/assets/9608067a-c0a1-4572-87cc-d606c239c72a)

## Verify Python Version 
```
python3 --version
```

## Install Dev. tool 
```
sudo apt install python3-dev python3-venv build-essential -y
```
![image](https://github.com/user-attachments/assets/5a138859-9483-4028-b676-c942a3b5c034)


## Install Yarn
```
sudo apt-get update && sudo apt-get install -y curl gnupg apt-transport-https && curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add - && echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list && sudo apt-get update && sudo apt-get install -y yarn
```


### Check version
```
yarn --version
```


# Get HuggingFace Access Token 
[Hugging Face Security Tokens](https://huggingface.co/docs/hub/en/security-tokens)

  - Sign up , verify and create account
  - Go to Menu, click the ```Access token ```
  - Create a ```Write access``` token and DONE! 

![image](https://github.com/user-attachments/assets/9222d990-1d24-4d96-a7d7-00ca9da9b9b5)


# Clone RL-Swarm Repo 
### RL Swarm is an open source system for peer-to-peer reinforcement learning over the internet. Running a swarm node allows you to train your personal model against the swarm intelligence. 

```
git clone https://github.com/gensyn-ai/rl-swarm
```

### Navigate in 
```
cd rl-swarm
```

![image](https://github.com/user-attachments/assets/d033e5ce-ff44-49d8-97c6-c0268061aeb3)


### Install screen 
```
sudo apt install screen -y
```

### Create screen for process  
```
screen -S rlswarm
```

### Install and Run Swarm 
```
python3 -m venv .venv
source .venv/bin/activate
./run_rl_swarm.sh
```

![2025-04-01_22h30_09](https://github.com/user-attachments/assets/a48558bd-9f88-4ac9-8c26-2b437ac2e5ac)


---

## Wait till you see ```waiting for UserData.json to be created```
![image](https://github.com/user-attachments/assets/0eb0a771-3afb-4640-a8a3-38aac53f0aeb)

No open Browser and Input 
```http://localhost:3000/``` 

![2025-04-02_00h05_35](https://github.com/user-attachments/assets/fbe91e2a-9072-40ca-9794-77753969963c)




## I faced some random funny issues I tried to force solve and discover I just leave them and wait.😒
![image](https://github.com/user-attachments/assets/8ebf1da6-22f5-4a3c-812b-0d5b0d5bcec8)



## Would you like to push to the RL swarm, select ```Y``` and paste token from HuggingFace
![2025-04-02_09h41_54](https://github.com/user-attachments/assets/3ac0514c-a7cc-4743-8389-f3246d5888a0)

## Take note of Username

## Access ```.pem``` file and save ```swarm.pem```  
![image](https://github.com/user-attachments/assets/95b41c10-30e1-4904-bca3-103b7d13361d)

  - Click ```Home``` and ```select username``` , select ```rl-swarm```  ans save the ```swarm.pem```

![image](https://github.com/user-attachments/assets/16fc0e76-be7e-4a54-90d1-5c5579fb2c87)


---


## Search your Username after some time here [Visit Gensyn Dashboard](https://dashboard.gensyn.ai/)


# Official guide 
[Check Official guide](https://github.com/gensyn-ai/rl-swarm?tab=readme-ov-file)


