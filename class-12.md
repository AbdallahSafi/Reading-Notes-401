# OAuth

__Why is authentication important?__  
This is an important part of protecting a users info. If we do not use good authentication, then the wrong people could sign into other user accounts.

__Why should we be careful about storing a user’s password?__  
It is important becuase a user might have sensitive information that they are storing on the site or app. By asking for sensitive information, it is important to be responsible with the passwords to keep the users safe.  

__What is the difference between hashing and encryption?__  
Something that is encrypted can be decrypted. Something that is hashed cannot be unhashed, it is a one way function. Hashing is more secure than encryption.  


__What is the difference between encryption and encoding?__   
Encoding can be reversed by the same algorithm, but encryption needs a key to be reversed, so encryption is more secure than encoding.  


__What is a token used for?__  
A token is used to authenticate a a user.  

## Vocabulary Terms  
  
|Term | Definition |  
|---|---| 
| authentication | Verifying a user's identity by requiring pre-required details. |
| authorization | The process of allowing a user access to a resource. |
| encryption | The translation of data to another form so that only a secret key or password can read it.| 
| hashing | The conversion of one value to another. This is done to make data like passwords difficult to decipher.| 
| session | Interactions with a website that take place in a given time frame. | 
| cookie | A small amount of data that is stored by the web browser to so a website can remember information about you. h | 
| token | With token based authentication, the user state is stored on the client. The data is encrypted in a JWT. The server then validates the JWT. | 
| Basic Auth | An authentication built into HTTP , where the authorization header contains the word basic followed by a space and an encoded string of `username:password` |
| encoding | The process of converting one code of data to another. It goes from something a user can understand to something less clear. | 
| secret | This ia a secret that only the application and authorizaiton server know. It should be random enough that it can not be guessed. |
| cryptography | Protecting information by transforming it into a format that can not be easily understood. | 