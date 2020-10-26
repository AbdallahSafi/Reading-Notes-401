# Redux - Asynchronous Actions 

__How granular should your reducers be?__  
There should be a separate reducer function for each slice of data. They are combined before being put into the store.  

__Pro or Con - multiple reducers can "fire" when a commonly named action is dispatched__  
This is a Con because you may fire off reducers that you did not intend.  

__Name a strategy for preventing the above__  
You can use more specific names to make sure that the right action fires the right reducer at the correct time.

|Term | Definition |  
|---|---|
| store | This holds the state of the application. This can only be changed when actions are dispatched to the store. |
| combined reducers| This takes all the reducer functions from an app and combines them to pass to createStore.|