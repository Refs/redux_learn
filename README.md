# redux_learn

## course1 

the first principle of redux -- everything that changes in your application , including the data and the ui stata , is contained in a single object , we call the stata or the stata tree.

## course2 

the second principle of Redux -- the state is read only . the only way to chage the state tree is by dispathing an action. an action is a plain javascript object describing in the minimal way what changed in the application. whether it is initiated by a network request or by user interaction, any data that gets into the redux application gets there by actions 