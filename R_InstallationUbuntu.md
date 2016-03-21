# 在UBUNTU安裝R與RStudio(以14.04 LTS Long Term Support為例)

## 安裝R-Base

- 安裝VIM編輯軟體

```shell
sudo apt-get install vim
```

- 編輯/etc/apt/sources.list

```shell
sudo vim /etc/apt/sources.list
```

- 在/etc/apt/sources.list文件的最下方加入CRAN Mirror的entry(按i可以寫入文字):

```shell
deb http://cran.csie.ntu.edu.tw/bin/linux/ubunmtu trusty/
```

這裡以台灣大學資工系的CRAN Mirror為例，你可以置換成你偏愛的[CRAN Mirror](https://cran.r-project.org/mirrors.html)。
如果你的UBUNTU版本不是14.04，請根據版本調整:

版本|Entry
15.10|deb http://cran.csie.ntu.edu.tw/bin/linux/ubuntu wily/
15.04|deb http://cran.csie.ntu.edu.tw/bin/linux/ubuntu vivid/
12.04|deb http://cran.csie.ntu.edu.tw/bin/linux/ubuntu precise/

加完之後按`:wq`存檔並離開。

- 加入UBUNTU在CRAN的Key至系統

```shell
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E084DAB9
```

- 安裝R-base

```shell
sudo apt-get update
sudo apt-get install r-base
sudo apt-get install r-base-dev
```

- 在/etc/apt/sources.list文件的最下方加入UBUNTU Mirror

```shell
deb http://ftp.ubuntu-tw.net/mirror/ubuntu/ trusty main 
deb-src http://ftp.ubuntu-tw.net/mirror/ubuntu/ trusty main 
```

這裡以Ubuntu-TW為例，你可以置換成你偏愛的[UBUNTU Mirror](https://launchpad.net/ubuntu/+archivemirrors)。

## 安裝RStudio

- 至[Download RStudio](https://www.rstudio.com/products/rstudio/download/)下載最新版本的RStudio。

![]()

- 開始安裝

```shell
cd 
```

## 資料來源
- [CRAN](https://cran.r-project.org/)