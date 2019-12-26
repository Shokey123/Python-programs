# Python-programs
#No of notes issued by ATM machine 




amount= int(input("Enter amount:"))
note_count = 0

if amount%10 != 0:
    print("Amount should be multiple of Rs 10.")
else:
    
    
    if amount>=2000:
        print("Number of 2000 notes:",amount//2000)
        note_count += amount//2000
        amount = amount%2000
    else:
        print("2000 notes are not available")
        
 
    if amount>=1000:
        print("Number of 1000 notes:",amount//1000)
        note_count += amount//1000
        amount = amount%1000
    else:
        print("1000 notes are not available")

    if amount>= 500:
        print("Number of 500 notes:",amount//500)
        note_count += amount//500
        amount = amount%500
    else:
        print("500 notes are not available")
        
    
    if amount>= 100:
        print("Number of 100 notes:",amount//100)
        note_count += amount//100
        amount = amount%100
    else:
        print("100 notes are not available")
    
    
    if amount>= 50:
        print("Number of 50 notes:",amount//50)
        note_count += amount//50
        amount = amount%50
    else:
        print("50 notes are not available")
        
    if amount>= 10:
        print("Number of 10 notes:",amount//10)
        note_count += amount//10
        amount = amount%10
    else:
        print("10 notes are not available")
    print("Total Notes:",note_count)   
