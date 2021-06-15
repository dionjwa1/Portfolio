# Class 1 notes
- Event Loop: Executes taks in a queue. 

- Solving Problems: Don't try to overcomplicate problem solving. Start with the simpilest terms or processes, and evolve the solving from there. Trying to grab too much at once, or solve the entire problem in one swoop often leads to failure. 

- Super Mario Effect: choose to approach learning in a way that is motivating for you. THe mindset used to learn best should be applied when receiving new information. 

- The 5 Whys: ask why 5 times (sometimes more, sometimes less) Get to the RCA of the problem before you stop asking why. 

- Act like you make $1k an Hour: your time is valuable. Treat it as such, and ensure others treat your time with respect, too. 



## Useful Code Tips


## Vocab

- Array.map() = a callback function that creates a new array based on the argument entered as the mapping value and is applied to every value in the old array.  

- Array.reduce() = `Subtracts all values in an array starting from the left of the array. 

- superagent() = function loginUserInternal(user, request) {
  return new Promise((resolve,reject) => {
    let auth = {};
    request
      .post('/users/login')
      .send({
        username: user.username,
        password: user.password_decoded,
      })
      .expect(200)
      .end(onResponse);
    function onResponse(err, res) {
      if(err) return reject(err)
      auth.id = res.body.id;
      auth.token = res.body.token;
      auth.tokenExpires = res.body.tokenExpires;
      resolve(auth)
    }
  })
}`

- Promises = A promise is a gaurantee exectution made by your code that will operate asynchronous, but ultimately will conclude the promised coded operation. 

- CB Functions = CB functions can be both asynchronous or synchronous. However, they are mostly used as asynchronous operations. 

### Works Cited
 - I was helped with info or data from W3 Schools, and MOD Dev, Stackoverflow