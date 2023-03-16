# Message-encryption
message encryption in python ( 16 mar 2023 )


Write a python program for encrypting a message sent to you by your friend. The logic of encryption 
should be such that, for a the output should be z. For b, the output should be y. For c, the output should 
be x respectively. Also, the whitespace should be replaced with a dollar sign. Keep the punctuation 
marks unchanged.

Input Sentence: I want to become a Data Scientist.

Encrypt the above input sentence using the program you just created.

Note: Convert the given input sentence into lowercase before encrypting. The final output should be 
lowercase 





                    def Mymessage(message):
    
                        keywords = {'a': 'z', 'b': 'y', 'c': 'x', 'd': 'w', 'e': 'v', 'f': 'u', 'g': 't', 'h': 's', 'i': 'r', 'j': 'q',
                                   'k': 'p', 'l': 'o', 'm': 'n', 'n': 'm', 'o': 'l', 'p': 'k', 'q': 'j', 'r': 'i', 's': 'h', 't': 'g',
                                   'u': 'f', 'v': 'e', 'w': 'd', 'x': 'c', 'y': 'b', 'z': 'a', ' ': '$'}
    
                        encrypted_mess = ""
                        for char in message:
                            if char in keywords:
                                 encrypted_mess += keywords[char]
                            else:
                                 encrypted_mess += char
                        return encrypted_mess


                    # message=input("Enter your message:  ")
                    message="I want to become a Data Scientist"

                    encrypted_mess = Mymessage(message)
                    print("Encrypeted message: ",encrypted_mess)
                    
                    
                    
                    
                    
                    
