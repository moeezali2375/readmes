# EC2 Setup for nvim

## Step 1: Install nvim

```bash
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.tar.gz
sudo rm -rf /opt/nvim
sudo tar -C /opt -xzf nvim-linux-x86_64.tar.gz```

## Step 2: Add nvim to .bashrc

```bash
echo "export PATH="$PATH:/opt/nvim-linux-x86_64/bin"" >> ~/.bashrc
```

