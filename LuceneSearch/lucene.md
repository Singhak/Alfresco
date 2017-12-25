# USE these query in Alfresco Node browser
- ### all content in dictionary folder which is modified in The entire month of December, 2017.
	>PATH:"/app:company_home/app:dictionary/*" AND @cm\:modified:2017-12

- ### all content in dictionary folder which is modified in month of NOW

	> PATH:"/app:company_home/app:dictionary/*" AND @cm\:modified:NOW

- ### all content in dictionary folder which is modified in month of 25 December and year 2017

	> PATH:"/app:company_home/app:dictionary/*" AND @cm\:modified:2017-12-25
	
- ### all content in dictionary folder which is modified From the start of 2017 till the end of the 25th day of December.

	> PATH:"/app:company_home/app:dictionary/*" AND @cm\:modified:[2017 TO 2017-12-25]
	
- ### all content in dictionary folder which is modified From the start of 2017 till month of December.

	> PATH:"/app:company_home/app:dictionary/*" AND @cm\:modified:[2017 TO 2017-12]
	
- ### all content in dictionary folder From which is modified the start of 2017 till the end of the 25th day of December.

	> PATH:"/app:company_home/app:dictionary/*" AND @cm\:modified:[2017 TO 2017-12-25]

- ### all content in dictionary folder Which is modified TODAY

	> PATH:"/app:company_home/app:dictionary/*" AND @cm\:modified:TODAY
	
- ### all content in script folder whose name after "." has "j"

	> PATH:"/app:company_home/app:dictionary/app:scripts/*" AND @cm\:name:*.j*

- ### all content in script folder whose name start with "j" 
	> PATH:"/app:company_home/app:dictionary/app:scripts/*" AND @cm\:name:j*

- ### all content in script folder whose name contain "." 
	> PATH:"/app:company_home/app:dictionary/app:scripts/*" AND @cm\:name:*.*
	
- ### all content in script folder
	> PATH:"/app:company_home/app:dictionary/app:scripts/*"
	

	
### Try with yourself it will give interesting results:

> PATH:"/app:company_home/app:dictionary/*"  +@cm\:modified:TODAY

> +PATH:"/app:company_home/app:dictionary/*"  +@cm\:modified:TODAY

> -PATH:"/app:company_home/app:dictionary/*"  +@cm\:modified:2017-12-22

> -PATH:"/app:company_home/app:dictionary/*"  -@cm\:modified:2017-12-22

> PATH:"/app:company_home/app:dictionary/*"  -@cm\:modified:2017-12-22
