# ToshitaiRecorder

This is a script that records "Seven Eleven Presents - Sakura Toshitai Onishi"

Official website: [セブン-イレブン presents 佐倉としたい大西 | インターネットラジオステーション＜音泉＞](https://www.onsen.ag/program/toshitai/)

**DO NOT SHARE ANY VIDEOS** which recorderd by this script.

**ONLY FOR PERSONAL USE.**

## Requirements

You need to install [ffmpeg](https://www.ffmpeg.org/).

Also, if you are Windows user, you need an environment that can execute bash script.
I recommend [Git for Windows](https://gitforwindows.org/).

## Usage

1. Clone this repository.
1. Give `ToshitaiRecorder` a permission of execution.
1. Run **on Tuesday**.
1. Wait.

```
git clone git@github.com:mystasly48/ToshitaiRecorder.git
cd ToshitaiRecorder
chmod u+x ./ToshitaiRecorder
./ToshitaiRecorder
```

## Customize

You can use cron to schedule to run the script.

But the recording file will be saved in a directory **where the script was executed**.

It means the script tries to save the file on `/usr/bin/` but it doesn't have permission to write and the recording will be failed.


You can configure the path where the recording files will be saved, by editing `path=""` variable [on line 29](https://github.com/mystasly48/ToshitaiRecorder/blob/master/ToshitaiRecorder#L29).

For example
```
path="/mnt/c/radio/ToshitaiRecorder/"
```

Also, an example setting of cron is
```
28 23 * * 2 /mnt/c/radio/ToshitaiRecorder/ToshitaiRecorder
```

## Original

[mystasly48/ToshitaiRecorder.sh on GitHub Gist](https://gist.github.com/mystasly48/07b4b4167cfbb91c97bec846dd2c5c3d)

