# WebSVF-backend

## Description

This is a simple NodeJS CLI tool to easily install WebSVF and run it.

## Installation

Download the **[binary (websvf-create-analysis-1.0.0.tgz)](https://github.com/SVF-tools/WebSVF/releases/download/0.9.1/websvf-create-analysis-1.0.0.tgz)** file

Extract it:
```
tar zxvf websvf-create-analysis-1.0.0.tgz
```

Test it:
```
cd package
sudo npm link
```

Run it:
```
--- COMING SOON ---
```

## Usage

### 1. Install WebSVF Extensions and Dependencies (SVF, LLVM, Clang...)

```
sudo create-analysis -i [-u user]
```

#### **`-i`** or **`--install`** :

To install WebSVF and all its dependencies

#### **`-u user`** or **`--user user`**: 

Where the `--user` flag indicates that a String is being provided which is the `user` for which WebSVF should be installed. If the user is not specified with the `--user` flag then the user is prompted with a list of users to select from.

### 2. Generate Analysis for LLVM Bitcode (.bc) file

Generate the bitcode file for your program or project then run the following command from the same directory as the .bc file or specify the directory of the .bc file.

```
create-analysis -g [bc-file-directory]
```