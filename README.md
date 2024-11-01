# 文字列を実行する

[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=Arithmos-tools_string_exec_test&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=Arithmos-tools_string_exec_test)
[![Security Rating](https://sonarcloud.io/api/project_badges/measure?project=Arithmos-tools_string_exec_test&metric=security_rating)](https://sonarcloud.io/summary/new_code?id=Arithmos-tools_string_exec_test)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=Arithmos-tools_string_exec_test&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=Arithmos-tools_string_exec_test)
[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=Arithmos-tools_string_exec_test&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=Arithmos-tools_string_exec_test)

## 概要

このプロジェクトは、`main.cpp` ファイルを使用して、文字列データを実行可能にする方法を示しています。このプログラムは、Linuxのシステムコール `mprotect` (ID: `0xA`) を利用し、データの実行権限を変更します。

## 要件

- Linuxカーネル (バージョン 6.11)

## 使用方法

1. `main.cpp` をコンパイルします。

    ```bash
    make
    ```

2. 実行します。

    ```bash
    ./target
    ```

このプログラムは、指定されたメモリ領域に対して `mprotect` システムコールを使用し、データが実行可能になるように権限を変更します。

## ファイル構成

- `main.cpp` : プログラムのメインソースコード。
