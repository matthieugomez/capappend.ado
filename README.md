## description

`batchappend.ado` solves the following problem. When appending a bunch of `.dta` created from `xls`, two variables may have the same name but differing types (string vs numerical). In this case, `append` throws an error. With the `force` option, `append` converts the string observations to missing values. Instead, the command `capappend` converts the numerical observations to strings.

## installation

```
net install capappend , from(https://github.com/matthieugomez/stata-capappend/raw/master/)
```

If you have a version of Stata < 13, you need to install it manually

1. Click the "Download ZIP" button in the right column to download a zipfile. 
2. Extract it into a folder (e.g. ~/SOMEFOLDER)
3. Run

	```
	cap ado uninstall capappend
	net install capappend, from("~/SOMEFOLDER")
	```
