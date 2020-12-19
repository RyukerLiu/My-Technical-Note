# 如何使用 plantuml

## Online Server

最容易使用是線上編輯模式，若有安全性和資訊保密的考量，則不適用。

[plantuml online server](http://www.plantuml.com/plantuml/uml/SoWkIImgAStDuNBAJrBGjLDmpCbCJbMmKiX8pSd9vt98pKi1IW80?switch)

## Local Server with docker and VSCode Extension

1. 可使用 docker 啟動 plantuml local server 於 http://localhost:8080

```shell
docker run -it --rm -p 8080:8080 plantuml/plantuml-server:jetty
```

2. 接著使用 Visual Studio Code 並安裝下列 Extension

    [vscode-plantuml](https://github.com/qjebbs/vscode-plantuml)

3. 調整VSCode user setting, and configure like:
```
"plantuml.server": "http://localhost:8080",
"plantuml.render": "PlantUMLServer",
```

參考連結

- [UML 組件圖 component ](http://plantuml.com/zh/component-diagram)
- [甘特圖 Gantt ](http://plantuml.com/zh/gantt-diagram)

###### tags: `Note`