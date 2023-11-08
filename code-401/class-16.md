# Class 16

## Sources

- [Reading: What is Serverless Computing?](https://www.ibm.com/topics/serverless)
- [Video: What is Serverless](https://www.youtube.com/watch?v=vxJobGtqKVM)

## Additional Resources

- [venv](https://docs.python.org/3/library/venv.html)
- [Vercel](https://vercel.com/docs/getting-started-with-vercel)
- [http.server](https://pymotw.com/3/http.server/index.html)
- [Requests](https://requests.readthedocs.io/en/latest/)
- [Python & APIs](https://realpython.com/python-api/)

## Bookmark and Review
- [Serverless Functions](https://vercel.com/docs/functions/serverless-functions)
- [Effective Python Environment](https://realpython.com/effective-python-environment/)

## Notes

## Reading Questions

1. What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?
> It looks like serverless computing resembles FaaS (function as a service) with additional benefits. Key characteristics and benefits include having the  infrastructure managed and maintained exclusively by the cloud provider allowing developers the ability to focus solely on the code and business logic. It is also platform independent so they can also write the application in any language using any framework that they are most comfortable with. There is a huge cost savings since there is no idle capacity and computing resources are utilized on demand, and scales to zero when not in use. Traditional server-based architecture have a huge upfront cost because they have to house, build, and maintain the server themselves, as well as have in-house experts on the payroll in case something goes wrong. 

2. How can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?
> The steps to get started is to first sign up for an account. Next, create a new project either by deploying a template or importing and deploying an existing project. Then, a domain needs to added. Final step is to collaborate which I think it means to add collaborators to the project. 

3. What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?
> API stand for application program interface. They allow different systems to communicate. They can be utilized by requesting a key from the API of choice and using HTTP get request methods to make requests for info or data from that API.  
4. What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library?
> According to its documentation, 'Requests is an elegant and simple HTTP library for Python, built for human beings'. I think that means it's easy to use and powerful. 

`import requests`
`response = requests.get("http://randomuser.me/api/")`


## Things I want to learn more about
- Kubernetes
- Docker
- SOAP vs. REST vs. GraphQL
- FaaS