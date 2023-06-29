# Perseus Build
This repo template will allow you to build Perseus using Github Actions. This will helps people who don't want to setup build environments on their machines.

## Notes
- The script requires download link, to make it fits CN version and for some cases, apkpure don't have the latest version.
- Under **NO CIRCUMSTANCES** any APKs will be uploaded to this repository to avoid DMCA.
- This is only tested on CN version, if you need other version,you need to do some change.
- I don't use github frequently. So I won't do any Technical support for this.

## How to setup
1. Create a new PRIVATE repository using this repository as a template ([Guide](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)).
2. Go to newly created repo Settings > Actions > General > Workflow permissions > Set Read and Write permission.
3. Find the download link yourself and replace the link in line 29 in patch_perseus.sh (if you need versions of other regions, you also need to change the package name, Ctrl+H would do the job.)

## How to build
1. Go to Actions -> All workflows -> Perseus Build
2. Run the workflow
3. Download the APKs from the draft releases
