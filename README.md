# Perseus Build
This repo template will allow you to build Perseus using Github Actions. This will helps people who don't want to setup build environments on their machines.

## Notes
- Under **NO CIRCUMSTANCES** any APKs will be uploaded to this repository to avoid DMCA.
- This repo was designed for two circumstances: CN version and other regions when apkpure doesn't have the latest version.
- The ability to edit the code is required
- I don't use github frequently. So I won't do any Technical support for this.

## How to setup
1. Create a new PRIVATE repository using this repository as a template ([Guide](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template)).
2. Go to newly created repo Settings > Actions > General > Workflow permissions > Set Read and Write permission.
3. Find the download link yourself and replace the link in line 29 in patch_perseus.sh (if you need versions of other regions, you also need to change the package name, Ctrl+H would do the job.)

## How to build
1. Go to Actions -> All workflows -> Perseus Build
2. Run the workflow
3. Download the APKs from the draft releases

## How to change region
1. This project can only patch .apk file, if you want to patch .xapk file, uncommennt these 2 lines in patch_perseus.sh and  change the suffix in wget:![image](https://github.com/CapitalGrin/AzurLaneBiliBili-Perseus/assets/109933411/c1d4ea1e-c00f-49d5-969e-11054d6ae8c6)
![image](https://github.com/CapitalGrin/AzurLaneBiliBili-Perseus/assets/109933411/8d721bae-34d8-4edf-8944-fc95e308ab13)
2. change the download link here in patch_perseus.sh . And make sure the link is not Disposable or Dynamic.(high lighted part)
![image](https://github.com/CapitalGrin/AzurLaneBiliBili-Perseus/assets/109933411/07f37070-015d-4b40-84e1-b23a1f6c856c)
3. replace ALL the packge name in patch_perseus.sh , Ctrl+F would do the work.(Don't change the suffix though)
![image](https://github.com/CapitalGrin/AzurLaneBiliBili-Perseus/assets/109933411/d91800e7-ca14-4b91-9931-07acc28a5d56)
