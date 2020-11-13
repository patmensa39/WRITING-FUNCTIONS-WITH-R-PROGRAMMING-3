# WRITING-FUNCTIONS-WITH-R-PROGRAMMING-3
Else statements , if else statement,  Loops, while loops , Nexted loops, Multiple loops 

### Functions 
myfun<- function(a=3, b=3, c=2) {

  a+b+c
  
}

myfun()

### Another example 

philant<- function(a=3, b=45, c=4) {

  a+b+c
  
}

philant()

### Another function but remember b will not work because  I did not call it it the function. 

accent1<- function(a,b){

  2*a
  
}

accent1(2,2000)

### Another function

accent<- function(a,b){
  x<-3+2
  
  y<-2*z
  
  z<- 5^4+ 10%%2
  
  a*x*y+z
  
}

accent(2,1)


### Another function by printing them individually before the main function

accent<- function(a,b){

  x<-3+2
  
  z<- 5^4+ 10%%2
  
  y<-2*z
  
  a*x*y+z
  
  print(x)
  
  print(y)
  
  print(z)
  
}

accent(2,1)


## Control structures. 
## If statements
score<-100

if(score>90){

  print("Philant is a good student", quote = FALSE)
  
}

maths<-100

English<-100

if(maths>90 && English>90){

  print("Philant will be academic legend")
  
}

## if else statements
score<-100

if(score>90){

  print("Philant is a good student", quote = FALSE)
  
} else {

  print("Philant is not a good student")
  
}
### Same but score changed
score<-70

if(score>90){

  print("Philant is a good student", quote = FALSE)
  
} else {

  print("Philant is not a good student")
  
}

## Another if else statement
maths<-100

English<-100

if(maths>90 && English>90){

  print("Philant will be academic legend")
  
} else {

  print("Philant is not an academic legend")
  
}

## Same code for if else statement but the maths and English changed. Remember this is a conditional statement.You can also change the values

maths<-10

English<-100

if(maths>90 && English>90){

  print("Philant will be academic legend")
  
} else {

  print("Philant is not an academic legend")
  
}

### Remember you can change the values of x, y, and z. 
x<-300

y<-200

z<-400

if(x>= 100 && x<200){

  print("x is in the hundreds")
  
}else {

  print("x is not in the hundreds")
  
}
if(y>=200 && y<300) {

  print("y is in the two hundreds")
  
} else {

  print("y is not in the two hundreds")
  
}
if(z>=300 && z<400){

  print("z is in the three hundreds")
  
}else {

  print("z is not in the three hundreds")
  
}


## Nested if statements.
## Nested if statement to if Philant can pay his rent in Winding Wood apartments

annual.income<-100000

if(annual.income>=80000){

  print("Philant can pay his rent")
  
}else if(annual.income>=55000 && annual.income<70000){

  print("Philant can somehow pay his rent")
  
}else {

  print("Philant cannot pay his rent")
  
}

## There are 13 ways to deny a diversity visa lottery winner a visa at the US embassy in Ghana. 
wrong.answers<-0

if(wrong.answers==0){

  print("You wil be given the visa")
  
} else if(wrong.answers<0 && wrong.answers<2){

  print("You are likely to be denied the visa")
  
} else{

  print("You will be dinied the visa")
  
}

## Ifelse statements. Lets assume Patrick will gives birth to a boy or a girl using modulo 5
patrick<-c(1:10)

ifelse(patrick%%5==0, "Patrick will give bith to a boy", "Patrick will give birth to a girl")



## Switch statements helps to select a statement.


switch(2,"Patrick", "Senyo","Mensah")


switch(1,"Patrick", "Senyo","Mensah")


switch(3,"Patrick", "Senyo","Mensah")


### this produce NULL

switch(4,"Patrick", "Senyo","Mensah")


### Another way.

switch("first.name", "last.name"= "Mensah", "middle.name"="Senyo", "first.name"="Patrick")


## For loop
### Examples


pat<-c(1:10)

for(i in pat){

print(i)

}
## Another way

pat<-c(1:10)

for(i in pat){

print(pat)

}

### Another way. 

kaywa<-5

for(i in seq(1:20)){

phil<-5*kaywa

}


phil

print(i)


kaywa<-5

for(i in seq(1:20)){

phil<-5*kaywa

}



### For loops to count the number of even numbers 

philant<-c(21,56,378,98,82,11,66, 100, 98,200,222,23)

count<-0

for(val in philant) {


if(val %% 2==0) count= count+1
}

print(count)

### For loop

luda<-c(1:20)

kay<-34

for (i in luda){

kay<-kay+i

}

kay

### Breaks 
### To stop at when is 100

pati<-seq(20,200)

for(i in pati){

if(i==100){

break

}

print(i)

}
### Next 
### To skip the value 

for(i in pati){

if(i==150){

next

}

print(i)

}

###While loop

dad<-1

while(dad<150){

print("May dad lives long")

dad=dad+1

}





### Looping in matrix

philant<-matrix(1:15, nrow = 3, byrow = FALSE)

for (i in philant) {

print(i)

}





### Nested loop

philant<-matrix(seq(2, 40, by=2),nrow=5, ncol=4, byrow = FALSE)

for(row in 1:nrow(philant)) {

for(col in 1:ncol(philant)) {

print(philant[row, col])

}

}



### Multiple loops

kk<-matrix(seq(2,200, by=14), nrow = 5, byrow = T)

for(i in seq_len(nrow(kk))){

for(j in seq_len(ncol(kk))){

print(kk[i,j])

}

}







