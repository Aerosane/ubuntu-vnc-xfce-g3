# Examples `util-readme.sh`

Updated: 2022-09-11

***

**Warning**

It seems like the `publish` command is currently not always working. Some changes on the **Docker Hub** side seem to be the reason.  However, you can always copy the content generated by the `preview` command (`scrap-readme.md`) to the **Docker Hub** manually.

DEPRECATED: The 'publish' command is deprecated and it will be removed or replaced.

***

## Preparation

You have to have `curl` installed for this utility.

Open a terminal window and change the current directory to `utils`.

Then copy the secrets example file, modify the copy and source it:

```shell
### make a copy and then modify it
cp example-secrets-utils.rc secrets-utils.rc

### source the secrets
source ./secrets-utils.rc
```

Optionally you can provide the secrets as command line parameters.

You can also provide the secrets file as a command line parameter instead of sourcing it.

Embedded help describes the parameters:

```shell
./util-readme.sh -h
```

## Usage examples

```shell
./util-readme.sh --repo accetto/ubuntu-vnc-xfce-g3 --context=../docker/xfce -- preview
./util-readme.sh --repo accetto/ubuntu-vnc-xfce-g3 --context=../docker/xfce -- publish

./util-readme.sh --repo accetto/ubuntu-vnc-xfce-chromium-g3 --context=../docker/xfce-chromium -- preview
./util-readme.sh --repo accetto/ubuntu-vnc-xfce-chromium-g3 --context=../docker/xfce-chromium -- publish

./util-readme.sh --repo accetto/ubuntu-vnc-xfce-firefox-g3 --context=../docker/xfce-firefox -- preview
./util-readme.sh --repo accetto/ubuntu-vnc-xfce-firefox-g3 --context=../docker/xfce-firefox -- publish
```
