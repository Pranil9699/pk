let API_NINJAS='JilZxywCSNntIKDkl6GFnA==iiBGVzC7UF7cU4js'

  let name = 'golden retriever'
  let object={
    method: 'GET',
    headers: { 'X-Api-Key': `${API_NINJAS}`},
    contentType: 'application/json',
  }
  fetch('https://api.api-ninjas.com/v1/dogs?name=' + name,object).then((value)=>{
    return value.json();
  }).then((value)=>{
   
    for (const key in value) {
        
            const element = value[key];
            console.log(element)
            
        }
    });
