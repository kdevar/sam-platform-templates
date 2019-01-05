# sam-platform-templates

## Local Development
You will need to install your chosen language and sam

#### Install Golang
<a href="https://golang.org/dl/" target="_blank">Official installation guidelines</a>

or

```bash
brew upgrade
brew update
brew install go
```

#### Install SAM

```bash
brew upgrade
brew update
brew tap aws/tap
brew install aws-sam-cli
```

#### Install Docker
<a href="https://store.docker.com/editions/community/docker-ce-desktop-mac" target="_blank">Official installation guidelines</a>


## Add a skeleton Go Lambda

```
$ sam init -l  src/templates/sam-lambda-go/ -o stacks/
# prompt for project name
```

Here's an example of adding a new `foo_bar` lambda:

```
$ sam init -l src/templates/sam-lambda-go/ -o stacks/
$ make -f stacks/foo_bar/Makefile test
$ make -f stacks/foo_bar/Makefile build
```
