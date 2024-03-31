# About

- This is a TCP server built primarily with javaScript.
  - Utilizing node for the runtime enviroment.
  - Built within the HTTP protocol.

## Usage

**After cloning the repo verify that your in** `tcp-server-http`
**Ensure you have**`node (18)`**or better installed locally**

- To verify run: `which node`
  **For node installtion**:

> - Darwin/mac run:`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash`
> - Linux run:`curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash`
> - Windows run:`Set-ExecutionPolicy Bypass -Scope Process -Force;[System.Net.ServicePointManager]::SecurityProtocol= [System.Net.ServicePointManager]::SecurityProtocol -bor 3072;
iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'));`
>   **Then run `choco install nodejs`**

3. Then run `node app/main.js`

### Testing

- Once server is running, open another terminal. If in an IDE, then open local shell. If in local shell, open another shell
  - Then run: `nc localhost 4221`
  - Simultaneous request first run the `nc localhost 4221`, open another terminal and then run: `curl localhost:4221`
    - ** Server has been built to utilize the non-blocking functionality of node **
- To test sending content, within a file run `curl -vvv -d "Hello world!!!" localhost:4221/files/test-file.txt`

#### Built With

<p> 
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/bash/bash-original.svg" height="80" width="80" hspace="10px" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/nodejs/nodejs-original-wordmark.svg" height="80" width="80" hspace="10px" />
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/javascript/javascript-plain.svg" height="80" width="80" hspace="10px" />
</p>
