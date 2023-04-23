# tuto-github

## How to configure your git 

I am using `Git bash` as terminal.

## SSH key 

### Generate ssh key 

```shell
ssh-keygen -t ed25519 -C "your_email@example.com"
```

- Keep the default path.
- Enter your `Passphrase` 

### Add to ssh-agent

```shell
eval "$(ssh-agent -s)"
> Agent pid 59566
``` 

Add the key to ssh-agent 

```shell
ssh-add ~/.ssh/id_ed25519
```

### Add to your Github account 

Copy your key

```shell 
clip < ~/.ssh/id_ed25519.pub
```

On GitHub 
- access to your `settings`
- `Access` -> SSH-Key or GPG-Key
- Add new SSH-Key
- Add a `name` paste your key in `Key`
- Save 

> Github can ask to you to validate with your password

**You can used your SSH Key now!**



## How to start with git 

### From a fresh folder

Create a folder 

```shell
mkdir new_repository
```

Go to this folder 

```shell 
cd new_repository
```

Initialize git 

```shell
git init
```

You can verify if the folder `.git` exist

**Your repository has git**

### For an existing folder

run the following command *without ssh*

```shell 
git clone https://github.com/olarno/tuto-github.git
```

run the following command *with ssh*

```shell
git clone git@github.com:olarno/tuto-github.git
```


