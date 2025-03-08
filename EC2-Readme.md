# EC2 Setup

## nvim Setup

### Step 1: Install nvim

```bash
curl -LO https://github.com/neovim/neovim/releases/latest/download/nvim-linux-x86_64.tar.gz
sudo rm -rf /opt/nvim
sudo tar -C /opt -xzf nvim-linux-x86_64.tar.gz
```

### Step 2: Add nvim to .bashrc

```bash
echo "export PATH="$PATH:/opt/nvim-linux-x86_64/bin"" >> ~/.bashrc
```

### Step 3: Install Luarocks

```bash
sudo apt install luarocks
```

## NodeJS Setup

```bash
# Download and install nvm:
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.1/install.sh | bash

# in lieu of restarting the shell
\. "$HOME/.nvm/nvm.sh"

# Download and install Node.js:
nvm install 22

# Verify the Node.js version:
node -v # Should print "v22.14.0".
nvm current # Should print "v22.14.0".

# Verify npm version:
npm -v # Should print "10.9.2".

```

## PyEnv Setup

### Step 1: Install pyenv

```bash
curl https://pyenv.run | bash
```

### Step 2: Add pyenv to bashrc

```bash
echo -e 'export PYENV_ROOT="$HOME/.pyenv"
\nexport PATH="$PYENV_ROOT/bin:$PATH"' >> ~/.bashrc
echo -e 'eval "$(pyenv init --path)"\neval "$(pyenv init -)"' >> ~/.bashrc
```

### Step 3: Install Dependencies for Python

```bash
sudo apt update && sudo apt install -y \
    make build-essential libssl-dev zlib1g-dev \
    libbz2-dev libreadline-dev libsqlite3-dev \
    wget curl llvm libncursesw5-dev xz-utils tk-dev \
    libxml2-dev libxmlsec1-dev libffi-dev liblzma-dev
```

### Step 4: Install a python version

```bash
pyenv install <version>
```

### Step 5: Set that python to global

```bash
pyenv global <version>
```
