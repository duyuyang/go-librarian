# How to setup a webserver in go

Tutorial: https://www.lynda.com/Go-tutorials/Replacing-default-template-engine/516402/516855-4.html

## run the server

go run main.go

http://localhost:8080/

## setup webserver negroni

go get github.com/urfave/negroni

## Setup db

$ go get github.com/mattn/go-sqlite3

$ sqlite3 dev.db

sqlite> .schema

CREATE TABLE books(
pk integer primary key autoincrement,
title text,
author text,
id text,
classification text);

sqlite> select * from books;

sqlite> .exit

`alter the table`

sqlite> alter table books add column user varchar(255); 



## html template render

go get github.com/yosssi/ace

## http route

go get github.com/gorilla/mux

## db query

https://github.com/go-gorp/gorp

go get gopkg.in/gorp.v1

## manage sessions

go get github.com/goincremental/negroni-sessions

## encrypt user

go get golang.org/x/crypto/bcrypt


## Wrapping up

`Goji`
https://github.com/zenazn/goji


`Martini`

github.com/go-martini/martini


`Revel`

github.com/revel/revel
github.com/revel/cmd/revel

## migrate to postgresql

`postgresql driver`
github.com/lib/pq