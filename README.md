<h1 align="center"> PingPong Reward Program </h1>

> We are going to run a PingPong Mining Node in this tutorial
>
> This tutorial is for installing on Linux
>
> The stronger your server is, the more you will farm

<h1 align="center"> PingPong x MorphL2 Campaign </h1>

> Before we start the mining node, there is now a live Ping Pong x MorphL2 campaign that you can participate-in just by claiming and staking tokens without running a node
>
> 1- Connect your wallet: https://app.pingpong.build/points?invite_code=yc76BLjH
>
> 2- Claim a daily mLPT & mGRT token faucet on Holesky Network in `Points` tab
>
> 3- You can do `Boost Your Rewards` section to increase your daily faucet
>
> 4- Bridge tokens to MorphL2: https://app.pingpong.build/bridge
>
> 5- Stake on MorphL2: https://app.pingpong.build/markets
>
> Now you are farming PPP + Morph points - the more you stake daily, the more you farm points
>
> Now let's go for PingPong Mining Program

<h1 align="center"> PingPong Mining Program </h1>

## 1- Register
> Connect your Email in the [dashboard](https://harvester.pingpong.build/)

## 2- Install
```console
# Downlaod linux files
wget https://pingpong-build.s3.ap-southeast-1.amazonaws.com/linux/latest/PINGPONG
```

```console
# Install and update your linux packages
sudo apt-get update
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common screen

# Downlaod Docker packages
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

# Add docker to your packages
sudo add-apt-repository \
   "deb [arch=amd64] https://download.docker.com/linux/ubuntu \
   $(lsb_release -cs) \
   stable"

# Update packages
sudo apt-get update

# Install Docker
sudo apt-get install docker-ce

# Start Docker
sudo systemctl enable docker

sudo systemctl start docker

# Give Permissions to Docker
sudo usermod -aG docker $USER

# Test Docker
docker run hello-world
```

## 3- Run
```console
# Start a screen
screen -S pong
```

> Add a device in [dashboard](https://harvester.pingpong.build/devices)
>
> Copy your Device ID
>
> ![Screenshot_1](https://github.com/0xmoei/pingpong-mining/assets/90371338/1b8a0269-8cf9-4eec-bab7-66744a933ffb)


```console
# Replace DEVICE_ID with your ID you copied
chmod +x ./PINGPONG && ./PINGPONG --key DEVICE_ID
```

> Ctrl+A+D to minimze your screen
>
> Check the results here ( You are farming AIOZ , MASQ , TITAN tokens and PPP points)
>
> ![Screenshot_2](https://github.com/0xmoei/pingpong-mining/assets/90371338/0d1a0882-4063-4f5a-b27d-d8bb8d07fe4b)
>
>  You can now add more to run on more devices
>
## Tokenomics
![9d48f7371467ee7f1dde092f753575d6e823b623](https://github.com/0xmoei/pingpong-mining/assets/90371338/89053f18-368c-4d5f-b4c1-e53f274be08f)

![Screenshot_3](https://github.com/0xmoei/pingpong-mining/assets/90371338/b00abff6-a794-4176-838b-fb23e8b41d95)

Thanks Rues for the detailed guide - Follow [0xMoei](https://x.com/0xMoei) on Twitter

