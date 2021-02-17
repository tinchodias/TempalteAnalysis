# Template Analysis

This is a template to start your project using [this specialized tool](https://github.com/tinchodias/youtube-notes).

## File Structure

The `json` file contains the model, and it's the only important file to version along the analysis process.
```
├── README.md            <-- This file
├── tool                 <-- The tool is cloned here
│   ├── server.js        <-- The HTTP server
│   └── spa-client        
│       ├── index.html   <-- Web app's starting point
│       ├── css
│       ├── js
│       └── partials
├── .env                 <-- Configuration for the tool (db path, port number)
└── analysisDb.json      <-- Videos and marks model
```

## How to Install

1. Ensure you have a recent [nodejs](https://nodejs.org/).
2. Open a terminal, change directory to some appropriate subdirectory of your user (e.g. `Documents`). Then:
```
git clone https://github.com/tinchodias/TemplateAnalysis.git
cd TemplateAnalysis
git clone https://github.com/tinchodias/youtube-notes.git tool
cd tool
ln -s ../.env .
npm install
```

## How to Launch

1. Open a terminal, change directory to `TemplateAnalysis/tool`.
2. Run `npm start`.
3. Open browser on http://localhost:3000.

You can find a small usage guide [here](https://github.com/tinchodias/youtube-notes/blob/master/README.md).
