# aws-cloudops-workshop by sbaruffi@

### Setup:

#### Install Hugo:
On a mac:

`brew install hugo`

On Linux:
  - Download from the releases page: https://github.com/gohugoio/hugo/releases/tag/v0.37
  - Extract and save the executable to `/usr/local/bin`

#### Clone this repo:
From wherever you checkout repos:
`git clone https:/github.com/dixonaws/aws-cloudops-linux`

#### Clone the theme submodule:
`cd aws-cloudops-linux`

`git submodule init`

`git submodule update --checkout --recursive`

#### Install node packages:
`npm install`

#### Run Hugo locally:
`npm run server`
or
`npm run test` to see stubbed in draft pages.

#### View Hugo locally:
Visit http://localhost:8080/ to see the site.

#### Making Edits:
As you save edits to a page, the site will live-reload to show your changes.
