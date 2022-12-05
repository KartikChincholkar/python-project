# python-project
# It finds the prime and composite numbers between any 2 given inputs
A=input('Enter the value of A:')
B=input('Enter the value of B:')
c=0
p=0

if (A.isdigit() and B.isdigit()) or (A.lstrip('+').isdigit() and B.isdigit()) or (B.lstrip('+').isdigit() and A.isdigit() ) :

    a=int(A)
    b=int(B)
    if a<b:
        for a in range(a,b+1):
            x=1
            count=0
            while(x<=a):
                if a%x==0:
                    count=count+1
                x=x+1
            if count==2:
                p=p+1
                print("{} is prime number".format(a))
            elif count>2:
                c=c+1
                print("{} is composite number".format(a))
            else:
                print()
        print("{} prime and {} composite number in range.".format(p,c))
    else:
        d=0
        d=a
        a=b
        b=d
        for a in range(a,b+1):
            x=1
            count=0
            while(x<=a):
                if a%x==0:
                    count=count+1
                x=x+1
            if count==2:
                p=p+1
                print("{} is prime number".format(a))
            elif count>2:
                c=c+1
                print("{} is composite number".format(a))
            else:
                print()

        print("{} prime and {} composite number in range.".format(p,c))
elif (A.lstrip('-').isdigit() and B.isdigit()) or (B.lstrip('-').isdigit() and A.isdigit()) or (A.lstrip('+').isdigit() and B.isdigit()) or (B.lstrip('+').isdigit() and A.isdigit() ) :
    a=int(A)
    b=int(B)
    if a<b:
        for a in range(a,b+1):
            x=1
            count=0
            while(x<=a):
                if a%x==0:
                    count=count+1
                x=x+1
            if count==2:
                p=p+1
                print("{} is prime number".format(a))
            elif count>2:
                c=c+1
                print("{} is composite number".format(a))
            else:
                print()
        print("{} prime and {} composite number in range.".format(p,c))
    else:
        d=0
        d=a
        a=b
        b=d
        for a in range(a,b+1):
            x=1
            count=0
            while(x<=a):
                if a%x==0:
                    count=count+1
                x=x+1
            if count==2:
                p=p+1
                print("{} is prime number".format(a))
            elif count>2:
                c=c+1
                print("{} is composite number".format(a))
            else:
                print()

        print("{} prime and {} composite number in range.".format(p,c))

elif  type(A)==str or type(B)==str or A.isdecimal() or B.isdecimal():

    print(" can not find prime and composite number between this range.")

else:
    print(" can not find prime and composite number between this range.")

