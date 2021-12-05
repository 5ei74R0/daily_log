# 2021/12/4 (SAT)

<div class="date_jumper">
  <a class="link_wrapper" href="./3rd.md"><div class="button">go to the previous day</div></a>
  <a class="link_wrapper" href="./5th.md"><div class="button">go to the next day</div></a>
</div>

## Univ.
### courses
no courses

## Other Activities
### Install Docker on WSL2 Ubuntu 20.24 LTS  
  ```sh
  ~$ sudo apt update
  ~$ sudo apt upgrade
  ~$ sudo apt install curl
  ~$ sudo apt install apt-transport-https
  ~$ sudo apt-get remove docker docker-engine docker.io containerd runc
  ~$ sudo apt install ca-certificates gnupg lsb-release
  ~$ curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker-archive-keyring.gpg
  ~$ echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive-keyring.gpg] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null
  ~$ sudo apt update
  ~$ sudo apt install docker-ce docker-ce-cli containerd.io
  ~$ sudo apt install docker-compose
  ~$ sudo groupadd docker
  ~$ sudo usermod -aG docker $USER
  ~$ newgrp docker
  ~$ service --status-all  // [ - ]  docker
  ~$ sudo service docker start
  ~$ service --status-all  // [ + ]  docker
  ~$ docker run hello-world
  ~$ docker container ls
    // CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
  ~$ docker image ls
    // REPOSITORY    TAG       IMAGE ID       CREATED        SIZE
    // hello-world   latest    feb5d9fea6a5   2 months ago   13.3kB
  ```

### setting the formatter clang-format on VSCode
write below on setting.json
```json
{
  // C, C++
  "C_Cpp.clang_format_style": "{ BasedOnStyle: LLVM, BreakBeforeBraces: Attach, IndentWidth: 4 }",
}
```

### Reading papers, articles, books, codes
- read [WSL2のUbuntuでDockerを使う](https://zenn.dev/sprout2000/articles/95b125e3359694#11.-docker-engine-をインストールする)
- read [Install Docker Engine on Ubuntu](https://docs.docker.com/engine/install/ubuntu/)
- read [Post-installation steps for Linux](https://docs.docker.com/engine/install/linux-postinstall/)
- read [vscodeのC++用コード整形設定(clang-formatの設定)](https://fastapple.hatenablog.com/entry/vscode/clang-format)
- [Advancing mathematics by guiding human intuition with AI](https://www.nature.com/articles/s41586-021-04086-x)
  - revolution by AI on mathematics field!?

## Memo, Feelings, Thoughts
no contents
