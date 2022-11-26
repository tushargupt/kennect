# Question:  Write and submit code to set up a handler for a focus event on an input element having an id name which is a direct child of an element having id john.
# When run, the handler should add the HTML class shape to all elements having an HTML class important which are direct children of an element having id john.
# The event should not propagate beyond the handler

Answer: $("div#john .important").classList.add(“shape”)

# Question:  Explain JWT in approx and provide its top 3 benefits.

Answer: JWT(JSON Web Token) is an open standard used to share information between two parties securely — a client and a server. In most cases, it’s an encoded JSON containing a set of claims and a signature. It’s usually used in the context of other authentication mechanisms like OAuth, and OpenID to share user-related information. It’s also a popular way to authenticate/authorize users in a microservice architecture.

Benefit of JWT

1. JWT is a stateless authentication mechanism as the user state is never saved in the database. As JWTs are self-contained, all the necessary information is there, reducing the need of going back and forward to the database. With JWT we don't need to query the database to authenticate the user for every API call.
 
2. JWT is compact. Because of its size, it can be sent through an URL, POST parameter, or inside an HTTP header.
 
3. We can authorize only the requests we wish to authorize. Cookies are sent for every single request.
 
# Question: Given a number x, finds out if it is a prime number or not, use javascript and find out the difference between the Next prime number after x and x.

Answer: 

const num = parseInt(prompt('Enter number: '));
const isPrime = (num) => {
   let sqrtnum = Math.floor(Math.sqrt(num));
   let prime = num !== 1;
   for(let i = 2; i < sqrtnum + 1; i++){
      if(num % i === 0){
         prime = false;
         break;
      };
   };
   return prime;
}
const nextPrime = () => {
  let nu = num
   while(!isPrime(++nu)){
   };
   return nu - num;
};
console.log(isPrime(num));
console.log(nextPrime(num));

