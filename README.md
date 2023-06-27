# Gerzhan Go Application

[github.com/gerzhan/gerzhan-go-application](https://github.com/gerzhan/gerzhan-go-application)

## Создание приложения на языке `Go`

- подготовка директории для размещения кода

```bash
# создать директорию для приложения
$mkdir gerzhan-go-application
# перейти в директорию
$cd gerzhan-go-application
```

- регистрация репозитория на `GitHub` [github.com/gerzhan/gerzhan-go-application](https://github.com/gerzhan/gerzhan-go-application)

- инициализация `Go` модуля приложения

```bash
$go mod init github.com/gerzhan/gerzhan-go-application
# просмотр сгенерированного файла
$cat go.mod
module github.com/gerzhan/gerzhan-go-application

go 1.20
```

## Создание файла `main.go` и запуск приложения

```go
package main

import "fmt";

func main() {
	fmt.Println("Hello Word!")
}
```

```bash
$go run ./main.go
```

## Сборка приложения (исполняемого файла)

```bash
# -o [директория дял][имя файла приложения]
$go build -o gerzhan-go-application main.go
# запуск собранного приложения на macOS
$./gerzhan-go-application
Hello Word!
```
