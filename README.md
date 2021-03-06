# Search App task

An app to perform various optimzations on searching because an api can have latency.

- Performed debouncing which avoids calling function call again and again. It calls functions after specified amount of time after users stops writing.
- Checked if user has atleast typed 2 characters to call the api, which again helps to not call api for 1-2 characters.
- Cached the results on the FE for a particular query for some time, so that we don’t make an api call for the same query.
- Cancelling previous requests which are time consuming and calling current request because... continued... (below)
- Data can come asynchronously and we want data to render which is currently called by user rather than calling and rendering useless data.

## Setup

- Setup Node.js and editor on your PC

  - [Download node.js](https://nodejs.org/en/download)
  - [Setup Editor](https://docs.flutter.dev/get-started/editor?tab=vscode)

## Install

Some basic Git commands are:

```
$ git clone https://github.com/pratik9333/Search-app-task.git
$ cd Search-app-task/search-task
```

## Install dependencies

```
$ npm install or npm i
```

## Run app

```
$ npm start
```

### Code Formatter

- Add a `.vscode` directory
- Create a file `settings.json` inside `.vscode`
- Install Prettier - Code formatter in VSCode
- Add the following snippet:

```json
{
  "editor.formatOnSave": true,
  "prettier.singleQuote": true,
  "prettier.arrowParens": "avoid",
  "prettier.jsxSingleQuote": true,
  "prettier.trailingComma": "none",
  "javascript.preferences.quoteStyle": "single"
}
```
