# Browser CTL MCP Server 

<p align="center">
  <a href="https://www.youtube.com/@BitEval">
    <img src="https://github.com/biteval/browser_ctl/blob/main/static/biteval_logo.jpeg" alt="BitEval">
  </a>
</p>


Browser CTL is a MCP server built on Python Playwright, providing a suite of tools that enable AI agents to control and interact with web browsers , this simple version use chrome browser.

# Exposed Tools:

## 1. execute_javascript

Execute JavaScript code in real-time browser using Playwright's evaluate method and return the script's result.

## 2. go_to_url

Visit a target url in real-time browser.

## 3. sleep_for

Browser sleep for a random seconds between begin and end .

## 4. close_browser

Close the opened browser.

## 5. open_browser

Open browser in real-time.



# Default log

This MCP server start with info log level by default:


```
#Configure logging
logging.basicConfig(
    level=logging.INFO, format="%(asctime)s - %(levelname)s - %(message)s"
)
```

# Default End Point

```
http://127.0.0.1:8001/sse

```


# INSTALL

First, clone this repo:

```
git clone https://github.com/biteval/browser_ctl.git

```

Move to the main dir:

```
cd browser_ctl

```

Now, let’s install uv and set up our Python project and environment:


## Linux:

```
curl -LsSf https://astral.sh/uv/install.sh | sh

```

## Windows:

```
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"

```


## Now, let’s set up our project:
 

```
uv init

```

```
uv venv

```


## Create virtual environment and activate it


## Linux:

```
source .venv/bin/activate

```

## Windows:

```
.venv\Scripts\activate

```


## Install dependencies

```
uv add "mcp[cli]" httpx playwright

```


## Download playwright browser binaries

```
python -m playwright install

```


## Start the Browser CTL MCP Server

```
python browser_ctl.py

```


## Contributions Are Welcome!

Your expertise and ideas can make a significant impact on this project. Thanks!


## Learn More

Visit our YouTube channel to learn how  to create AI agents:

[![Watch](https://img.youtube.com/vi/VIDEO_ID/0.jpg)](https://www.youtube.com/@BitEval)
  

