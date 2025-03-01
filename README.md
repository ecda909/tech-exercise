## TL500 Mono Repo

This monorepo holds the content for the TL500 (aka DO500). The structure is roughly as follows 
```bash
...
├── README.md
├── docs
│   ├── 1-the-manual-menace
│   ├── ...
│   ├── facilitation
│   └── slides
├── pet-battle
│   ├── stage
│   └── test
├── quick-starts
│   ├── README.md
│   ├── ...
├── tekton
│   ├── ...
├── ubiquitous-journey
    └── ...
```
whereby
* `docs` - contains the student and teacher guides for the technical exercises as well as the classroom activities. The `slides/content` are written in markdown and automatically published to the site when pushed to main.
* `pet-battle` - contains the application configs used by the tech exercise
* `ubiquitous-journey` -  contains a lightweight fork of the rht-labs ci/cd stack
* `tekton` - contains the OpenShift pipeline definitions used in the tech exercise.


### 🏃‍♀️ Running the docs & slides site locally
To launch the slides, ensure you have NodeJS installed or run it in a NodeJS container if you prefer.
```
npm i docsify-cli -g
docsify serve ./docs
```

* Open the browser to http://localhost:3000 to view the tech exercise.
* Open the browser to http://localhost:3000/slides to view the slides.

## 🎃 Contribution
Pull requests welcome 🎃

Changes approved and pushed to main will automatically be published to the docs site
